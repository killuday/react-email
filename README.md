# React Email Library

📧 A modern and efficient way to create beautiful email UIs using React, Next.js, and TypeScript.

## Features

✨ Create stylish and responsive email interfaces.
📥 Support for receiving and displaying emails.
💌 Compose and send emails with ease.
📤 Manage sent items and drafts.
🔒 Secure and user-friendly authentication system.
📦 Easily customizable and extendable.

## Installation

To get started with the React Email library, follow these steps:

# Manual Setup Guide for React Email Starter 🚀

Follow these steps to set up a brand-new folder with React Email:

## Step 1: Create Directory

Create a new folder called `react-email-starter` and initialize a new npm project:


mkdir react-email-starter
cd react-email-starter  
npm init

## Step 2: Install Dependencies

npm install react-email @react-email/button @react-email/html -E

## Step 3: Add Scripts
{
  "scripts": {
    "dev": "email dev --dir src/emails"
  }
}
## Step 4: Include Email Template
```bash
import { Button } from '@react-email/button';
import { Html } from '@react-email/html';
import * as React from 'react';

export default function Email() {
  return (
    <Html>
      <Button
        pX={20}
        pY={12}
        href="https://example.com"
        style={{ background: '#000', color: '#fff' }}
      >
        Click me
      </Button>
    </Html>
  );
}
```
## Step 5: Run Locally
npm run dev
## Step 6: See Changes Live
Visit http://localhost:3000 in your web browser, and you can edit the index.tsx file to see the changes live.
