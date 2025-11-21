# API Contracts - EndToEndLabCR Landing Page

## Overview

This document will contain API contract specifications when the backend is implemented. If starting without a backend, this section serves as a placeholder for future API design.

---

## REST API Endpoints (To Be Implemented)

### Base URL

```
Production: https://api.endtoendlabcr.com
Staging: https://api-staging.endtoendlabcr.com
Local: http://localhost:8000
```

### Authentication

- JWT token-based authentication for admin endpoints
- Public endpoints require no authentication

---

## Public Endpoints

### GET /api/events

**Description**: Retrieve list of events  
**Authentication**: None required  
**Query Parameters**:

- `status` (optional): "upcoming" | "past"
- `type` (optional): "workshop" | "webinar" | "hackathon" | "meetup"
- `limit` (optional): number of results (default: 20)
- `offset` (optional): pagination offset

**Response**: 200 OK

```json
{
  "events": [...],
  "total": 42,
  "limit": 20,
  "offset": 0
}
```

### GET /api/events/{id}

**Description**: Get specific event details  
**Authentication**: None required

---

### GET /api/projects

**Description**: Retrieve featured projects  
**Authentication**: None required

---

### GET /api/contributions

**Description**: Retrieve recent community contributions  
**Authentication**: None required

---

### POST /api/contact

**Description**: Submit contact form  
**Authentication**: None required

**Request Body**:

```json
{
  "name": "string",
  "email": "string",
  "subject": "string",
  "message": "string",
  "inquiry_type": "general | partnership | support"
}
```

---

### POST /api/subscribe

**Description**: Subscribe to newsletter  
**Authentication**: None required

---

## Admin Endpoints (Future)

### Authentication Required

- POST /api/auth/login
- POST /api/events (Create)
- PUT /api/events/{id} (Update)
- DELETE /api/events/{id} (Delete)

---

**Note**: Detailed API specifications will be added when backend implementation begins.
