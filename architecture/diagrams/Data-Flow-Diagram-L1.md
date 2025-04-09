```mermaid
%%{init: {'theme': 'default', 'themeVariables': { 'background': '#ffffff' }}}%%
flowchart TD
    P1(("Passengers")) -- Journey Requests & User Data --- PS["Passenger Services"]
    TD(("Transit Drivers")) -- Location & Status Updates --- VS["Vehicle Services"]
    AD(("Admin Staff")) -- System Management & Updates --- AMS["Administration Services"]
    TC(("Traffic Control Center")) -- Road Events & Conditions --- TMS["Traffic Management Services"]
    
    PS -- User Account Data --- DS1[("User & Ticket Data")]
    PS -- Journey Planning Requests --- VS
    VS -- Vehicle Location & Status --- DS2[("Transportation Operations Data")]
    VS -- Service Alerts --- PS
    PS -- Ticketing & Payment Data --- AMS
    AMS -- System Updates & Reports --- DS3[("System Configuration Data")]
    AMS -- Schedule & Service Management --- DS2
    TMS -- Traffic Conditions & Disruptions --- DS2
    TMS -- Route Adjustments --- VS
    VS -- Performance Metrics --- AMS
    
    PS:::process
    VS:::process
    AMS:::process
    TMS:::process
    P1:::entity
    TD:::entity
    AD:::entity
    TC:::entity
    DS1:::datastore
    DS2:::datastore
    DS3:::datastore
    
    classDef process fill:#f9f,stroke:#333,stroke-width:2px
    classDef entity fill:#bbf,stroke:#333,stroke-width:2px
    classDef datastore fill:#dfd,stroke:#333,stroke-width:2px
