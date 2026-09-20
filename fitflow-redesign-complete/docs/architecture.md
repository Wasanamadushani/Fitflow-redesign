# High-Level Architecture

See `architecture-diagram.png`.

## Components
- React Native / React Native Web client
- API Gateway
- Node.js/NestJS backend services
- Python/FastAPI AI microservice
- PostgreSQL system of record
- Firebase Firestore/Realtime Database for social real-time features
- Redis cache
- Firebase Cloud Messaging

## Critical data flows
1. Personalized workout: Client → API Gateway → Workout Service → AI Service → PostgreSQL/Redis → Client.
2. Social sharing: Client → Social Service → Firebase → real-time listeners → followers; notifications through FCM.
3. Nutrition tracking: Client → object storage → Nutrition Service → AI vision service → PostgreSQL → dashboard.

## Security
TLS, Firebase JWT verification, PostgreSQL row-level security, Firestore rules and signed image URLs.

## Scalability
Stateless backend services, horizontal scaling, PostgreSQL read replicas, managed Firebase real-time infrastructure and Redis caching.
