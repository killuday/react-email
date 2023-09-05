# React Email Library

📧 A modern and efficient way to create beautiful email UIs using React, Next.js, and TypeScript.

## Features

#### ✨ Create stylish and responsive email interfaces.
#### 📥 Support for receiving and displaying emails.
#### 💌 Compose and send emails with ease.
#### 📤 Manage sent items and drafts.
#### 🔒 Secure and user-friendly authentication system.
#### 📦 Easily customizable and extendable.
#### 💡 Bonus: Make it responsive effortlessly with Tailwind CSS!

## Installation

To get started with the React Email library, follow these steps:

# Manual Setup Guide for React Email Starter 🚀

Follow these steps to set up a brand-new folder with React Email:

## Step 1: Create Directory

Create a new folder called `react-email-starter` and initialize a new npm project:

```shell
mkdir react-email-starter
cd react-email-starter  
npm init
```
## Step 2: Install Dependencies
```shell
npm install @react-email/components
```
## Step 3: Add Scripts
```shell
  "scripts": {
    "dev": "email dev --dir src/emails"
  }
```
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
## Make it Responsive with Tailwind CSS
```bash
npm install @react-email/tailwind -E

```
### Add the component around your email body content.
```bash
import { Button } from '@react-email/components';
import { Tailwind } from '@react-email/tailwind';

const Email = () => {
  return (
    <Tailwind
      config={{
        theme: {
          extend: {
            colors: {
              brand: '#007291',
            },
          },
        },
      }}
    >
      <Button
        href="https://example.com"
        className="bg-brand px-3 py-2 font-medium leading-4 text-white"
      >
        Click me
      </Button>
    </Tailwind>
  );
};

```
## Step 5: Run Locally
```shell
npm run dev
```
## Step 6: See Changes Live
Visit http://localhost:3000 in your web browser, and you can edit the index.tsx file to see the changes live.
