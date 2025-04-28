## Use case name: Core Navigation Route Planning

| Field | Description |
|-------|-------------|
| Scenario: | User needs to plan a journey from their current location to a destination using public transit |
| Triggering event: | User opens app and enters destination address |
| Brief description: | Allows users to find optimal routes between locations using various public transportation options |
| Actors: | Transit app user |
| Related use cases: | Real-time tracking, Favorite locations |
| Stakeholders: | Passengers, Transit authorities, Transportation providers |
| Preconditions: | User has installed app, Location services enabled, Network connectivity available |
| Postconditions: | User has received route options with estimated arrival times and transit instructions |
| Flow of activities: | **Actor**<br>1. User enters destination address<br>2. User selects route preferences (fastest, fewest transfers, etc.)<br>3. User selects preferred route<br>4. User begins journey following instructions | **System**<br>1.1. System detects current location<br>2.1. System calculates available routes based on preferences<br>3.1. System displays detailed journey instructions<br>4.1. System updates route information in real-time |
| Exception conditions: | No network connectivity, Location services disabled, No available routes to destination |

## Use case name: Ticket Purchase and Validation

| Field | Description |
|-------|-------------|
| Scenario: | User needs to purchase and use a transit ticket for their journey |
| Triggering event: | User selects "Buy Ticket" option or approaches transit gate |
| Brief description: | Enables users to purchase, store, and validate digital tickets for various transit options |
| Actors: | Transit app user, Ticket inspector |
| Related use cases: | Payment processing, Ticket history |
| Stakeholders: | Passengers, Transit authorities, Payment processors, Ticket inspectors |
| Preconditions: | User has registered account with payment method, Network connectivity available |
| Postconditions: | User has valid ticket, Transaction recorded in system, Ticket can be validated by inspectors |
| Flow of activities: | **Actor**<br>1. User selects ticket type and quantity<br>2. User confirms purchase and payment method<br>3. User activates ticket when boarding<br>4. User presents ticket for validation when required | **System**<br>1.1. System displays available ticket options and prices<br>2.1. System processes payment securely<br>3.1. System generates valid ticket with QR code and timestamps<br>4.1. System verifies ticket validity and displays confirmation |
| Exception conditions: | Payment failure, Network connectivity issues during validation, Expired tickets |

## Use case name: System Administration

| Field | Description |
|-------|-------------|
| Scenario: | Transit administrator needs to update system information or manage user accounts |
| Triggering event: | Administrator logs into admin portal |
| Brief description: | Provides tools for administrators to manage transit schedules, pricing, user data, and system performance |
| Actors: | System administrator |
| Related use cases: | Data analytics, Service disruption management |
| Stakeholders: | Transit authorities, IT support team, Transportation providers |
| Preconditions: | Administrator has valid credentials, Secure network connection established |
| Postconditions: | System updates applied, Administrative tasks completed and logged |
| Flow of activities: | **Actor**<br>1. Administrator logs into secure portal<br>2. Administrator selects administrative function<br>3. Administrator makes necessary changes<br>4. Administrator confirms changes | **System**<br>1.1. System authenticates credentials and grants appropriate access level<br>2.1. System displays relevant tools and data<br>3.1. System validates changes for errors<br>4.1. System implements updates and logs all modifications |
| Exception conditions: | Authentication failure, System maintenance period, Data integrity issues |

## Use case name: Profile Personalization

| Field | Description |
|-------|-------------|
| Scenario: | User wants to customize app experience and accessibility settings |
| Triggering event: | User navigates to profile settings |
| Brief description: | Allows users to set preferences, accessibility options, and personalize their transit experience |
| Actors: | Transit app user |
| Related use cases: | Favorite locations, Notification settings |
| Stakeholders: | Passengers, Accessibility advocates |
| Preconditions: | User has registered account |
| Postconditions: | User preferences saved and applied across app experience |
| Flow of activities: | **Actor**<br>1. User navigates to profile settings<br>2. User modifies settings (language, theme, accessibility options)<br>3. User saves new preferences<br>4. User returns to app with personalized experience | **System**<br>1.1. System displays current preferences and customization options<br>2.1. System previews changes in real-time<br>3.1. System applies changes across all app functions<br>4.1. System maintains consistent experience based on preferences |
| Exception conditions: | Unsupported accessibility request, Settings sync failure |

## Use case name: Augmented Reality Navigation

| Field | Description |
|-------|-------------|
| Scenario: | User needs visual guidance for complex transit environments |
| Triggering event: | User activates AR mode at transit hub |
| Brief description: | Provides augmented reality overlays to guide users through stations, identify correct platforms, and facilitate transfers |
| Actors: | Transit app user |
| Related use cases: | Real-time tracking, Accessibility assistance |
| Stakeholders: | Passengers, Transit authorities, Station managers |
| Preconditions: | User has AR-capable device, Camera permissions granted |
| Postconditions: | User successfully navigates through transit environment following AR guidance |
| Flow of activities: | **Actor**<br>1. User activates AR navigation mode<br>2. User points camera at surroundings<br>3. User follows visual guidance<br>4. User reaches destination/platform | **System**<br>1.1. System accesses device camera and location services<br>2.1. System overlays directional arrows and information on camera view<br>3.1. System updates directions based on user movement<br>4.1. System confirms correct location with visual indicator |
| Exception conditions: | Low light conditions, Camera permissions denied, AR capabilities not supported by device |