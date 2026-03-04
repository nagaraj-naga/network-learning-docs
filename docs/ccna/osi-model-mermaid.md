# OSI Model (CCNA)

The OSI model defines 7 layers used to standardize network communication.

## OSI Layer Diagram

```mermaid
graph TD
    A[Layer 7: Application]
    B[Layer 6: Presentation]
    C[Layer 5: Session]
    D[Layer 4: Transport]
    E[Layer 3: Network]
    F[Layer 2: Data Link]
    G[Layer 1: Physical]

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
```

## Layer Responsibilities

| Layer | Name | Function |
|------|------|---------|
| 7 | Application | Network services to user applications |
| 6 | Presentation | Data translation, encryption |
| 5 | Session | Session management |
| 4 | Transport | End-to-end communication (TCP/UDP) |
| 3 | Network | Routing and logical addressing (IP) |
| 2 | Data Link | MAC addressing, switching |
| 1 | Physical | Transmission of raw bits |

## Packet Encapsulation Flow

```mermaid
flowchart LR
    App[Application Data]
    Seg[Segment]
    Pack[Packet]
    Frame[Frame]
    Bits[Bits]

    App --> Seg
    Seg --> Pack
    Pack --> Frame
    Frame --> Bits
```

This diagram represents how data moves down the OSI layers during encapsulation.
