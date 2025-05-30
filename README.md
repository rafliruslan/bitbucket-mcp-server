# Bitbucket MCP Server

A Model Context Protocol (MCP) server that provides integration with Bitbucket API for repositories, pull requests, and issues management.

## Features

- List and get repository details
- Manage pull requests (list, get details, create)
- Browse issues
- Full TypeScript support
- Error handling and validation

## Setup

1. Install dependencies:
```bash
npm install
```

2. Set up authentication:
```bash
cp .env.example .env
# Edit .env with your Bitbucket credentials
```

3. Build the project:
```bash
npm run build
```

4. Run the server:
```bash
npm start
```

## Authentication

Create a Bitbucket App Password:
1. Go to https://bitbucket.org/account/settings/app-passwords/
2. Create a new app password with required permissions:
   - Repositories: Read, Write
   - Pull requests: Read, Write
   - Issues: Read, Write

## Available Tools

### Repository Management
- `bitbucket_list_repositories` - List repositories in a workspace
- `bitbucket_get_repository` - Get repository details

### Pull Request Management
- `bitbucket_list_pull_requests` - List pull requests
- `bitbucket_get_pull_request` - Get pull request details
- `bitbucket_create_pull_request` - Create a new pull request

### Issue Management
- `bitbucket_list_issues` - List repository issues

## Development

```bash
# Development mode with auto-reload
npm run dev

# Type checking
npm run typecheck

# Linting
npm run lint
```