# mail
// using Twilio SendGrid's v3 Node.js Library
// https://github.com/sendgrid/sendgrid-nodejs
const sgMail = require('@sendgrid/mail');
sgMail.setApiKey(process.env.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);
const msg = {
  to: 'keisi.by@gmail.com',
  from: 'espesni@gmail.com',
  subject: 'Sending with Twilio SendGrid is Fun',
  text: 'and easy to do anywhere, even with Node.js',
  html: '<strong>and easy to do anywhere, even with Node.js</strong>',
};
sgMail.send(msg);
