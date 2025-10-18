# Frontend (React + TypeScript)

This folder will hold the event-tracking web app.

## Purpose
Collect basic user events and send them to the Quarkus API endpoint.

## Planned Features
- User ID input field  
- "Track Purchase" button  
- Heartbeat event every 30 seconds  
- Event payload validation before sending  
- Configurable API base URL via .env file  

## Output
Each action triggers a POST request:
POST /api/event
{
  "eventId": "uuid",
  "userId": "abc123",
  "eventName": "track_purchase",
  "ts": "2025-10-17T14:00:00Z",
  "props": {"app": "web"}
}
