# PRAISE CAGE API TEST LOG

## OVERVIEW
- Tester: Tim Baines
- Testing Date: June 10, 2025
- Project: Praise Cage REST API Workshop
- Environment: Github Codespaces
- Testing Tools: Val Town

## Checkpoint 1: Form Submission
- **Status**: ✅ Pass
- **Verification Date**: June 10, 2025
- **Test Steps**:
  1. Created HTML form with proper action URL pointing to Val.town endpoint
  2. Submitted a form entry with praise text
  3. Confirmed JSON response was received containing the submitted praise
  4. Verified form submission worked without any client-side JavaScript

## Checkpoint 2: Server Rendering
- **Status**: ✅ Pass
- **Verification Date**: June 10, 2025
- **Test Steps**:
  1. Updated Val.town endpoint to return HTML instead of JSON
  2. Added "View Praises" button to index.html
  3. Clicked "View Praises" button and confirmed an HTML page with praises was displayed
  4. Submitted a new praise and verified redirect back to form page
  5. Confirmed server-side rendering of praise list was functioning correctly

## Checkpoint 3: Local API Server
- **Status**: ✅ Pass
- **Verification Date**: June 10, 2025
- **Test Steps**:
  1. Created `server.js` with Node.js HTTP server implementation
  2. Confirmed server successfully serves static HTML form from `/`
  3. Verified GET `/praises` endpoint returns HTML with current praise list
  4. Tested POST `/praises` endpoint by submitting new praise via form
  5. Confirmed in-memory storage is working by viewing updated praise list

## Checkpoint 4: Authentication
- **Status**: ✅ Pass
- **Verification Date**: June 11, 2025
- **Test Steps**:
  1. Installed all required dependencies (fastify and plugins)
  2. Successfully logged in with test credentials (username: "nic", password: "praisecage!")
  3. Added, updated, and deleted praises while logged in
  4. Tested logout and log back in functionality 
