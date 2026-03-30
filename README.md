# AWS Step Functions on Vercel

This project demonstrates how to implement AWS Step Functions patterns using Vercel serverless functions.

## Features

- **Sequential Step Execution**: `/api/step/[step]` simulates step functions using 307 redirects to chain API calls
- **Parallel Execution**: `/api/parallel` triggers multiple parallel requests
- **Configurable Delays**: Uses a delay utility to simulate processing time

## API Endpoints

- `GET /api/step/[step]?end=N` - Execute a step, redirects to next step until reaching `end`
- `POST /GET /api/parallel` - Trigger parallel step function executions

## Tech Stack

- Next.js 12
- React 17
- Vercel
