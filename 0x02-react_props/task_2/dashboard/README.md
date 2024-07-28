Create a NotificationItem.js
The Notifications component is repeating the same tags a lot. It will be hard to maintain and reuse. Let’s create a component to support the li generation.

Create a new component named NotificationItem:

it should render a li tag
the component accept three properties (type, html, and value)
type should be rendered with the data-notification-type attribute
value should be rendered within the tag
html should be rendered with the dangerouslySetInnerHTML attribute
Create a NotificationItem.test.js
Every component should be tested. Create a new NotificationItem.test.js file, and add the following checks:

Verify that the basic rendering of the component works without crashing
Verify that by passing dummy type and value props, it renders the correct html (for example: type=“default” and value=“test”)
Verify that by passing a dummy html prop, it renders the correct html (for example: html={{ __html: '<u>test</u>' }})
Modify Notifications.js
Import the new NotificationItem component in the Notifications.js file and replace the <li> tags with NotificationItem components.

Modify Notifications.test.js
Modify the Notifications.test.js file to change one of the check:

Instead of testing if the component renders li, check that the component renders NotificationItem elements
Add a test to verify that the first NotificationItem element renders the right html (note: this is usually not the best way to write tests, but sometimes necessary when you don’t control the child component)
Requirements:

At this point, reloading the App should display the exact same page as the last task
The console in your browser should not show any error or warning
Running the test suites, should show:
Test Suites: 7 passed, 7 total
Tests: 22 passed, 22 total
