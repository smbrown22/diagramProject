##### Flowchart that shows the process of how a random number game is played out 
```mermaid
flowchart TD
    X(Game Starts)
    X--> A[[Computer creates a number]]
    A --> B[User makes a guess]
    B --> C[/User makes an input/]
    C--> D[Input is too high]
    C --> E[Input is too low] 
    D --> B 
    E --> B
    C --> F[Input is the right number]
    F --> G(Game Ends)
```
##### Sequence diagram which shows the process of a DDoS attack 
```mermaid
sequenceDiagram
    actor Attacker
    participant BotNet
    participant WebServer
    participant Firewall
    Attacker ->> BotNet: Herds a group of devices afflicted by malware 
    BotNet ->> WebServer: Floods the bandwidth of the server, causing service to be denied to actual participants
    Firewall ->> BotNet: Attempts to keep unauthorized traffic out of the WebServer
```
##### Nike Store ERDiagram which shows the process of how something is ordered, and delivered 
```mermaid
erDiagram
PRODUCT ||--o{INVENTORY:   ifAvailableIn  
CUSTOMER ||--o{SALE: makesA
SALE ||--o{PRODUCT: contains 
INVENTORY ||--o{DELIVERS: yes
INVENTORY ||--o{REFUND: no
```