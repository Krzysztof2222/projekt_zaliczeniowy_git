```mermaid
graph TD
    subgraph Uzytkownik
        A[Fleet Manager<br/>Administrator]
    end

    subgraph Aplikacja[Aplikacja do zarządzania flotą]
        B[Monitorowanie pojazdów GPS]
        C[Panel Kontrolny<br/>Dashboard]
        D[Harmonogram serwisowy]
        E[Rejestr paliwa i kosztów]
        F[Tryb offline<br/>rejestracja danych bez sieci]
    end

    A --- B
    A --- C
    A --- D
    A --- E
    A --- F

    B <--> D
    E --> C
    E -.-> |wpływa na| D