# CS50W Project 3: Mail

Welcome to my CS50W Project 3 - Mail! This project implements a front-end for an email client, making API calls to send and receive emails.

## Demo

Watch the project demo on YouTube: [CS50W Project 3 Demo](https://youtu.be/AIDLfAxs1s8).

## Overview

The project focuses on creating a Single Page Application (SPA) using JavaScript, HTML, and SCSS for styling. The primary file for implementation is `inbox.js`. All the essential functionalities are implemented as per the project specifications, and SCSS is utilized for enhanced styling.

## Features

### Send Mail

- Implemented the functionality to send emails using a POST request to `/emails`.
- Email composition form includes fields for recipients, subject, and body.

### Mailbox

- Users can view their Inbox, Sent mailbox, or Archive.
- Utilizes a GET request to `/emails/<mailbox>` to retrieve emails for a particular mailbox.
- Displays mailbox names at the top of the page.
- Each email is rendered in its own box with sender, subject, and timestamp.
- Unread emails have a white background, while read emails have a gray background.

### View Email

- Users can view the content of a selected email.
- Uses a GET request to `/emails/<email_id>` to retrieve the email.
- Displays sender, recipients, subject, timestamp, and body.
- Marks the email as read when clicked using a PUT request to `/emails/<email_id>`.

### Archive and Unarchive

- Allows users to archive and unarchive emails.
- Provides "Archive" and "Unarchive" buttons as needed.
- Uses a PUT request to `/emails/<email_id>` to mark an email as archived or unarchived.
- After archiving or unarchiving, loads the user’s inbox.

### Reply

- Enables users to reply to an email.
- Displays a "Reply" button when viewing an email.
- Clicking "Reply" pre-fills the email composition form with relevant details.

### Styling and Animations

- Utilized SCSS for enhanced styling, providing a more maintainable and modular stylesheet.
- Implemented basic animations to enhance the user interface.

## Implementation

The complete implementation can be found in the `inbox.js` file. The code is structured and commented for easy understanding.

Happy coding!
