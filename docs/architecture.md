# 🧱 Arquitectura del Sistema – Ichnos

```mermaid
flowchart LR

    U[Usuario]

    subgraph FRONTEND
        R[React App]
    end

    subgraph BACKEND
        C[Controllers]
        S[Services]
        R2[Repositories]
        E[Entities]
    end

    subgraph DATABASE
        DB[(SQLite DB)]
    end

    subgraph STORAGE
        OD[OneDrive Evidencias]
    end

    U --> R
    R -->|HTTP REST| C
    C --> S
    S --> R2
    R2 --> DB

    S -->|Archivos| OD
