# Authentication Guide for Gemini API using TypeScript

## Overview

This guide explains how to authenticate with the Gemini API using TypeScript. It focuses on three primary authentication methods: API keys, OAuth 2.0, and service accounts. 

## Prerequisites

- TypeScript Kernel is needed for this notebook to run properly.
- This notebook’s code can also be used for other TypeScript files and TypeScript projects.

## Dependencies

Ensure you have the following dependencies installed in your `package.json`:

```json
{
    "dependencies": {
        "axios": "^0.21.1",
        "debug": "^4.4.0",
        "dotenv": "^10.0.0",
        "express": "^4.21.2",
        "fs-extra": "^10.1.0",
        "googleapis": "^105.0.0"
    },
    "devDependencies": {
        "@types/express": "^5.0.0",
        "@types/node": "^22.13.9",
        "ts-node": "^10.4.0",
        "typescript": "^4.9.5"
    }
}
```

You can install the dependencies by running the following command:

```bash
npm install
```

## Configuration

Ensure your `tsconfig.json` is configured as follows:

```json
{
  "compilerOptions": {
    "rootDir": "./",
    "strict": true,
    "module": "commonjs",
    "lib": ["ESNext"],
    "target": "ESNext",
    "esModuleInterop": true
  }
}
```

You can set up the `tsconfig.json` manually or generate it using the following command:

```bash
npx tsc --init
```

## Authentication Methods

### 1. API Key Authentication

- **Setup**: Store your API key in a `.env` file.
- **Use**: Make authenticated requests using `axios` or another HTTP client.

### 2. OAuth 2.0 Authentication

- **Setup**: Configure OAuth credentials in a JSON file.
- **Use**: Handle OAuth flow using libraries such as `google-auth-library` and `express`.

### 3. Service Account Authentication

- **Setup**: Download the service account key file.
- **Use**: Authenticate server-to-server using the `google-auth-library`.

## Usage with Other TypeScript Projects

This notebook’s code can be easily adapted and reused for other TypeScript projects, including backend services or CLI applications. Simply copy the relevant parts of the authentication setup and modify the API request sections to fit the requirements of your project.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Required Links


1. [Install and use TypeScript Kernel in Jupyter](https://github.com/jupyter-xeus/xeus-cling)
2. [Google Auth Library for OAuth Authentication](https://www.npmjs.com/package/google-auth-library)
3. [Express (for handling OAuth flow)](https://expressjs.com/)
4. [Google Cloud Console (for managing projects, enabling APIs, and creating Service Accounts)](https://console.cloud.google.com/)
5. [Creating and Managing Service Accounts in Google Cloud](https://cloud.google.com/iam/docs/creating-managing-service-accounts)
6. [Google Cloud Service Account Documentation](https://cloud.google.com/iam/docs/service-accounts)
7. [Gemini API Documentation](https://docs.gemini.com/)
8. [Axios HTTP Client](https://axios-http.com/)
9. [TypeScript Compiler Options](https://www.typescriptlang.org/tsconfig)
10. [Node.js Package Manager (NPM)](https://nodejs.org/en/download/)