# Diagram przepływu aplikacji FocusFlow

```mermaid
flowchart TD
    A[Start] --> B[Logowanie / Rejestracja]
    B --> C{Masz konto?}

    C -- Tak --> D[Ustawienia]
    C -- Nie --> E[Rejestracja]

    D --> F[Personalizacja]
    E --> F

    F --> G[Panel główny]
    G --> H[Planowanie sesji]

    H --> I[Rozpoczęcie sesji]
    I --> J[Blokowanie rozpraszaczy]
    J --> K[Odliczanie czasu]

    K --> L[Przerwa Pomodoro]
    L --> M[Statystyki]

    M --> N[Wylogowanie]
    N --> O[Stop]
