
# Notification Microservice

The Notification Service Microservice is responsible for setting up event-based email notifications for applications within an organization. It allows administrators to configure notifications, manage applications, events, and notification types, and send messages to users based on various events. This readme provides an overview of the microservice's functionality, terminology, and user stories.

## Terminology
- Application: A product used by the organization.
- Event: An operation in an application that triggers email notifications to users (e.g., assigning a training to an employee).
- Notification Types: Different types of notifications triggered by an event (e.g., Trainee Notification, Manager Notification).
- Template: A blueprint for creating email messages with placeholders for metadata.
- Message: An email created using a template and sent to the user.
- Metadata: Information used to fill placeholders in templates (e.g., course title, course code, username)



## Features

- Log in to Notification Service UI
- Application:
    - Add Application
    - Modify application information.
    - Deactivate an application to prevent message sending.
    - Delete Application:
- Event:
    - Add Events to applications for triggering notifications.
    - Modify event information.
    - Deactivate an event to prevent message sending.
    - Delete Event:
- Notification:
    - Add Notification Types to the Events.
    - Update Notification information.
    - Delete Notifications
    - Deactivate Notifications to prevent sending message.
- Message:
    - Add custom messages using metadeta and tags to the enduser's notifications.
    - Suggesting Tags while writing notification message.

## Installation

To run this application, you have the option to use Docker for a streamlined setup or run individual npm scripts for the frontend and backend separately.

```shell
# Using Docker
docker build -t your-app-name .
docker run -p 80:80 your-app-name
```

### FrontEnd
    cd frontend
    npm install --force
    npm run start
    
### Backend
    cd backend
    npm install
    npm run start


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`SECRET_KEY`



