## Email Form Submission App

This is a simple Express and Node.js app that allows users to submit a form and sends an email using Gmail. The app requires a `.env` file with the following variables:

- `GMAIL_USER`: The email address to be used for sending emails.
- `GMAIL_PASS`: The password for the email address.
- `PORT`: The port on which the server will run.

### Data validation
This app uses [Joi](https://hapi.dev/module/joi/) to validate the data received from the form submission before sending the email, making sure that the required fields are present and in the correct format.
You can use Joi to create a schema for the form fields, such as the sender's email, name, subject, and message. Then, you can use the `validate()` function provided by Joi to validate the data against the schema. If the data is valid, it can proceed to send the email. If the data is not valid, you can return an error message to the user.

## Getting Started

1. Clone the repository to your local machine.
2. Run `npm install` to install the required dependencies including `@hapi/joi`.
3. Create a `.env` file in the root directory of the project and add the necessary variables.
4. Run `npm start` to start the server.
5. The app will be running on the port specified in the `.env` file.

## Notes

- This app only supports Gmail for sending emails.
- Make sure to use an email address that has access to less secure apps, otherwise the email sending will fail.

## Built With

- [Express.js](https://expressjs.com/) - Web framework for Node.js
- [Node.js](https://nodejs.org/) - JavaScript runtime
- [dotenv](https://www.npmjs.com/package/dotenv) - Library for loading environment variables from a .env file.
- [Nodemailer](https://nodemailer.com/about/) - Email sending library for Node.js
- [Joi](https://hapi.dev/module/joi/) - Object schema validation for Node.js

## Author

[Med Ben Malek](https://medbenmalek.me/)