# Functional Requirements

### 1. Route Planning & Navigation

- FR-1.1: The system must calculate routes between any two locations in Tirana and surrounding areas.
- FR-1.2: The system must allow users to set preferences (fastest route, fewer transfers, lowest cost).
- FR-1.3: The system must provide walking directions for first/last mile segments.
- FR-1.4: The system must recalculate routes when disruptions occur.
- FR-1.5: The system must save user's favorite routes and destinations.

### 2. Real-Time Tracking

- FR-2.1: The system must show current location of all public transport vehicles on a map.
- FR-2.2: The system must display estimated arrival times at stops.
- FR-2.3: The system must show passenger density levels on vehicles.
- FR-2.4: The system must send notifications about service disruptions.
- FR-2.5: The system must provide a service status dashboard.

### 3. Digital Ticketing & Payments

- FR-3.1: The system must allow purchase of single, multi-journey, and subscription tickets.
- FR-3.2: The system must generate QR codes for ticket validation.
- FR-3.3: The system must support multiple payment methods.
- FR-3.4: The system must provide family/group ticketing options.
- FR-3.5: The system must validate tickets at entry points.
- FR-3.6: The system must issue receipts for all transactions.

### 4. User Account Management

- FR-4.1: The system must allow users to create and manage accounts.
- FR-4.2: The system must store payment methods securely.
- FR-4.3: The system must track journey history.
- FR-4.4: The system must provide language options (Albanian, English, Italian).
- FR-4.5: The system must include accessibility features.

### 5. Administrative Functions

- FR-5.1: The system must provide fleet monitoring for operators.
- FR-5.2: The system must generate reports on passenger volumes and route performance.
- FR-5.3: The system must allow operators to update service information.
- FR-5.4: The system must collect and organize user feedback.
- FR-5.5: The system must provide tools for transit planning.

### 6. API & Integration

- FR-6.1: The system must provide APIs for third-party integration.
- FR-6.2: The system must incorporate tourism information.
- FR-6.3: The system must include special event transportation data.

# Non-Functional Requirements

### 1. Performance

- NFR-1.1: The system must support at least 40,000 concurrent users.
- NFR-1.2: The system must calculate routes in under 3 seconds.
- NFR-1.3: The system must maintain 99.9% uptime.
- NFR-1.4: The system must complete payment transactions in under 5 seconds.
- NFR-1.5: The system must maintain location accuracy within 10 meters.

### 2. Security

- NFR-2.1: The system must encrypt all personal and payment data.
- NFR-2.2: The system must comply with GDPR and Albanian data protection laws.
- NFR-2.3: The system must implement secure authentication for admin access.
- NFR-2.4: The system must time out sessions after 30 minutes of inactivity.
- NFR-2.5: The system must undergo regular security audits.

### 3. Usability

- NFR-3.1: The system must be usable without training.
- NFR-3.2: The system must meet WCAG 2.1 AA accessibility standards.
- NFR-3.3: The system must maintain consistent design across platforms.
- NFR-3.4: The system must allow one-handed operation for essential functions.
- NFR-3.5: The system must provide clear error messages.

### 4. Reliability

- NFR-4.1: The system must have maximum unplanned downtime of 1 hour per month.
- NFR-4.2: The system must implement automated backups.
- NFR-4.3: The system must function with reduced connectivity.
- NFR-4.4: The system must provide core features when offline.

### 5. Scalability

- NFR-5.1: The system must handle 50% annual growth in users.
- NFR-5.2: The system must support expansion to additional cities.
- NFR-5.3: The system must accommodate new transportation modes.

### 6. Maintainability

- NFR-6.1: The system must use modular architecture.
- NFR-6.2: The system must include comprehensive logging.
- NFR-6.3: The system must support configuration changes without redeployment.
- NFR-6.4: The system must follow documented coding standards.

### 7. Environmental

- NFR-7.1: Mobile apps must use no more than 5% battery per hour.
- NFR-7.2: The system must use energy-efficient infrastructure.
