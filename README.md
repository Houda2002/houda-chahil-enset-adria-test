# houda-chahil-enset-adria-test
# Architecture du projet 
            +------------------------+
            |   Frontend (Angular   |
            |      or React)        |
            +------------------------+
                     V
            +------------------------+
            |  Service Gateway       |
            | (Spring Cloud Gateway) |
            +------------------------+
                     V
            +------------------------+
            |  Service Discovery     |
            | (Eureka Server or      |
            |   Consul Discovery)    |
            +------------------------+
                     |
| +-------------+  +--------------+  +--------------+
| | Micro-service |  | Micro-service |  | Micro-service |
| |   Wallet      |  |   Transfert  |  |   Config     |
| | (Spring Boot) |  | (Spring Boot) |  | (Spring Cloud|
| +-------------+  +--------------+  |   Config or   |
|                                     | Consul Config)|
|                                      +--------------+
| +------------------------+
| |     Database (for     |
| |     Wallet Service)   |
| +------------------------+
| |     Database (for     |
| |   Transfert Service)  |
| +------------------------+

