
### Example Wiki Template in Azure DevOps

---

## Table of Contents

- [Overview](#overview)
- [Database](#database)
- [API](#api)
- [Website](#website)
- [Process Overview](#process-overview)

## Overview

A succinct synopsis of the Event Management System, elaborating on its purpose, entities, and primary functionalities.

## Database

### ER Diagram

Embed or link to the ER diagram visualizing the structure of the database.

### Data Types Overview

- **Events**: Stores information about each event.
- **Organizers**: Information concerning event organizers.
- **Attendees**: Details about individuals attending events.
- **Sponsors**: Data of organizations or individuals sponsoring events.

### Key Management

- Primary and Foreign keys
    - Events: EventID (PK), OrganizerID (FK)
    - Organizers: OrganizerID (PK)
    - Attendees: AttendeeID (PK), EventID (FK)
    - Sponsors: SponsorID (PK), SponsoredEvent (FK)

### Future Database Enhancements

Discussions on possible expansions or enhancements for the database.

## API

A breakdown of the API structure, specifying entities translated to C# objects, and their hierarchical structure.

## Website

### Storyboard

Visual representation (or link to) storyboards for each webpage.

### API Interaction

Example of how the website interfaces with the API, including request preparation, handling responses, and error management.

## Process Overview

### Example Workflow: Read Operation

1. **User Action**: User inputs search criteria and clicks "search".
2. **API Request**: The website sends a GET request to the API.
3. **Database Query**: API connects to the database, queries relevant data.
4. **API Response**: API retrieves data, converts to JSON, and sends it back.
5. **Display Data**: Website receives JSON, parses it, and dynamically populates the page.

---