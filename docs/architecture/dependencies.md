# Dependencies - EndToEndLabCR Landing Page

## Technical Dependencies

### Frontend Dependencies

#### Core Framework & Build Tools

- **React** (v18+) - UI library for component-based development
- **TypeScript** (v5+) - Type-safe JavaScript development
- **Vite** (v5+) - Build tool and development server
- **Node.js** (v18+ LTS) - JavaScript runtime for development

#### UI & Styling

- **Ant Design** (v5+) - UI component library
- **CSS/SCSS** - Styling and responsive design
- **Framer Motion** (v10+) - Animation library
- **styled-components** or **emotion** (Optional) - CSS-in-JS for theming

#### State Management & Routing

- **Redux Toolkit** (v2+) - State management
- **React Router** (v6+) - Client-side routing
- **Redux** (v5+) - Core Redux library

#### Data Fetching & Forms

- **Axios** or **fetch API** - HTTP client for API calls
- **React Query** (Optional) - Data fetching and caching
- **React Hook Form** - Form state management and validation
- **Yup** or **Zod** - Schema validation

#### Testing

- **Jest** (v29+) - Unit testing framework
- **React Testing Library** - Component testing
- **Vitest** (Alternative to Jest) - Vite-native test runner
- **Playwright** or **Cypress** - E2E testing

#### Utilities

- **date-fns** or **dayjs** - Date manipulation
- **react-i18next** - Internationalization (Phase 3)
- **lodash** or **lodash-es** - Utility functions

---

### Backend Dependencies (Optional)

#### Core Framework

- **FastAPI** (v0.109+) - Python web framework
- **Python** (v3.11+) - Programming language
- **Uvicorn** - ASGI server
- **Pydantic** (v2+) - Data validation

#### Database & ORM

- **PostgreSQL** (v14+) - Relational database
- **SQLAlchemy** (v2+) - ORM
- **Alembic** - Database migrations
- **asyncpg** - Async PostgreSQL driver

#### Authentication & Security

- **python-jose** - JWT token handling
- **passlib** - Password hashing
- **bcrypt** - Password hashing algorithm
- **python-multipart** - File upload support

#### API & Documentation

- **FastAPI** (built-in) - OpenAPI/Swagger documentation
- **CORS middleware** - Cross-origin resource sharing

#### Testing

- **Pytest** (v7+) - Testing framework
- **pytest-asyncio** - Async test support
- **httpx** - HTTP client for testing
- **pytest-cov** - Code coverage

---

### External Service Dependencies

#### Required Services

1. **GitHub API**

   - Purpose: Fetch organization projects, contribution data
   - Rate Limits: 5,000 requests/hour (authenticated), 60/hour (unauthenticated)
   - Mitigation: Implement caching (6-hour cache), use authenticated requests
   - Fallback: Static project data file

2. **Email Service Provider** (SendGrid, Mailgun, AWS SES)

   - Purpose: Send contact form submissions, confirmation emails, newsletters
   - Reliability: 99.9% uptime SLA
   - Fallback: Queue messages for retry if service is down

3. **Discord**
   - Purpose: Community chat and engagement
   - Dependency: Permanent invite link
   - Configuration: Server setup, roles, channels

#### Optional Services

1. **reCAPTCHA v3** (Google)

   - Purpose: Spam prevention on forms
   - Fallback: Honeypot field method

2. **CDN** (Cloudflare, AWS CloudFront)

   - Purpose: Global content delivery
   - Performance: Edge caching for static assets
   - Fallback: Direct hosting on Vercel/Netlify

3. **Video Hosting** (YouTube, Vimeo)
   - Purpose: Host event recordings
   - Dependency: Embed API support
   - Fallback: Direct video links

---
