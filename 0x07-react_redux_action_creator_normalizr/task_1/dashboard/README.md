Normalize a nested JSON

Copy over dashboard from the previous task into a task_1 directory at the root of the project

Modify src/schema/notifications.js to set up a schema using Normalizr

You’re going to use schema.Entity to create a 3 of entities.

The first one is an example the task will provide for you.

const user = new schema.Entity("users")

Create a message entity in a variable called message whose key is messages and set the idAttribute to the string guid in the options
Create a notification entity in a variable called notification whose key is notifications and set the definition of the entity as so:
author: user
context: message
