## UC-1. Use case name: Report Location/Status

| Field | Description |
|-------|-------------|
| Scenario: | Driver needs to report current vehicle location and operational status |
| Triggering event: | Driver logs into driver app at start of shift or route changes |
| Brief description: | Allows drivers to automatically or manually update their location and vehicle status for system tracking |
| Actors: | Transit vehicle driver |
| Related use cases: | Real-time tracking, Route monitoring, Schedule adherence |
| Stakeholders: | Drivers, Transit operations, Passengers, Fleet management |
| Preconditions: | Driver authenticated in system, GPS functionality available, Vehicle assigned to driver |
| Postconditions: | System updated with current vehicle location and status, Data available to operations and passengers |
| Flow of activities: | **Actor**<br>1. Driver logs into driver app<br>2. Driver confirms assigned route<br>3. Driver initiates route tracking<br>4. Driver manually updates status when needed (full, delayed, etc.) | **System**<br>1.1. System authenticates driver credentials<br>2.1. System loads route information<br>3.1. System begins automatic GPS tracking<br>4.1. System updates operations database with status changes |
| Exception conditions: | GPS signal loss, Network connectivity issues, Authentication failure, Wrong route assignment |

