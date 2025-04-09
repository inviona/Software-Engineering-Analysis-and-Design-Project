```mermaid
%%{init: {'theme': 'default', 'themeVariables': { 'background': '#ffffff' }}}%%
flowchart TD
    P1(("Passengers")) -- Journey Requests --- MP["Mobile Platform"]
    TD(("Transit Drivers")) -- Location Updates --- RTT["Real-time Tracking"]
    AD(("Admin Staff")) -- Administration Data --- AM["Admin Module"]
    CS(("City Services")) -- Road Data Event Info --- TM["Traffic Management"]
    MP -- Account Data --- DB1[("User Database")]
    MP -- Route Requests --- RP["Reporting"]
    MP -- Ticketing Data --- TS["Ticketing System"]
    MP -- "Real-time Vehicle Queries" --- RTT
    MP -- Service Disruption Alerts --- NA["Notification Agent"]
    RP -- Station/Route Queries --- DB2[("Transit Database")]
    RP -- Traffic Data --- TM
    RP -- Journey Plans --- DB3[("Journey Database")]
    RP -- Estimated Arrivals --- MP
    TS -- Payment Processing --- PP["Payment Processor"]
    TS -- Ticket Records --- DB4[("Ticket Database")]
    PP -- Transaction Records --- DB4
    RTT -- Vehicle Locations --- DB5[("Tracking Database")]
    RTT -- Delay Data --- NA
    RTT -- Vehicle Data --- DB2
    AM -- User Management --- DB1
    AM -- Service Updates --- NA
    AM -- Schedule Management --- DB2
    AM -- Report Generation --- RP
    NA -- Push Notifications --- MP
    NA -- Service Alerts --- DB6[("Notification Database")]
    TM -- Disruption Records --- DB7[("Traffic Database")]
    TM -- Route Impact Data --- RP
    RP -- Usage Statistics --- DB3
    RP -- Revenue Data --- DB4
    RP -- Performance Metrics --- DB5

     P1:::entity
     MP:::process
     TD:::entity
     RTT:::process
     AD:::entity
     AM:::process
     CS:::entity
     TM:::process
     DB1:::datastoren
     RP:::process
     TS:::process
     NA:::process
     DB2:::datastoren
     DB3:::datastoren
     PP:::process
     DB4:::datastoren
     DB5:::datastoren
     DB6:::datastoren
     DB7:::datastoren
    classDef process fill:#f9f,stroke:#333,stroke-width:2px
    classDef entity fill:#bbf,stroke:#333,stroke-width:2px
    classDef datastore fill:#dfd,stroke:#333,stroke-width:2px


