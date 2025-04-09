```mermaid
%%{init: {'theme': 'default', 'themeVariables': { 'background': '#ffffff' }}}%%
flowchart TD
    P1(("Passengers")) -- Journey Requests & User Data --> TPTS["Tirana Public Transportation MS"]
    TD(("Transit Drivers")) -- Location & Status Updates --> TPTS
    AD(("Admin Staff")) -- System Management & Configuration --> TPTS
    TC(("Traffic Control Center")) -- Road Events & Conditions --> TPTS
    
    TPTS -- Journey Plans & Service Alerts --> P1
    TPTS -- Route Updates & Instructions --> TD
    TPTS -- Reports & Operational Metrics --> AD
    TPTS -- Traffic Impact Acknowledgment --> TC
    
    TPTS:::central
    P1:::entity
    TD:::entity
    AD:::entity
    TC:::entity
    
    classDef central fill:#f5a442,stroke:#333,stroke-width:3px
    classDef entity fill:#bbf,stroke:#333,stroke-width:2px
