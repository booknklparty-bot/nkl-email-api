📧 NKL Entertainment – Email API

This is a lightweight serverless API for handling booking form submissions for NKL Entertainment.
When a visitor submits the booking form on the NKL website, this API sends the details directly to our email inbox via SendGrid.

🚀 Features

Accepts form submissions from the NKL Entertainment website

Sends email notifications via SendGrid

Serverless & scalable (deployable on Vercel, Netlify Functions, etc.)

Simple & secure (keeps email API keys private)

🛠 Tech Stack

Node.js

Express.js

SendGrid API

Serverless Deployment (Vercel recommended)

📂 Project Structure
.
├── api/
│   └── send-email.js   # Main serverless function
├── package.json
└── README.md

⚙️ Environment Variables

Before deploying, set these environment variables in your hosting platform:

Variable Name	Description	Example
SENDGRID_API_KEY	Your SendGrid API key	SG.xxxxxx
TO_EMAIL	Email address to receive submissions	booknklparty@gmail.com
FROM_EMAIL	Email address used to send messages	no-reply@nklentertainment.com
📬 API Endpoint

POST /api/send-email

Example Request:
{
  "name": "John Doe",
  "email": "john@example.com",
  "phone": "762-390-9143",
  "message": "I want to book a mascot for my kid's birthday."
}

Example Response:
{
  "success": true,
  "message": "Email sent successfully"
}

🚀 Deployment

Push this repo to GitHub.

Connect it to Vercel (or another serverless host).

Add environment variables in your host’s dashboard.

Deploy 🚀

📄 License

This project is private and intended for NKL Entertainment internal use.
