# Diagram przepływu – FocusFlow

Poniżej przedstawiono główny przepływ użytkownika w aplikacji FocusFlow.

```mermaid
flowchart TD
    A[Start] --> B[Logowanie / Rejestracja]
    B --> C{Masz konto?}
    C -- Tak --> D[Ustawienia]
    C -- Nie --> E[Rejestracja użytkownika]

    D --> F[Personalizacja sesji i przerw]
    D --> G[Integracja z kalendarzem]
    E --> F

    F --> H[Panel główny]
    G --> H

    H --> I[Planowanie sesji skupienia]
    I --> J[Wybór czasu i rozpraszaczy]
    J --> K[Rozpocznij sesję skupienia]

    K --> L[Blokowanie rozpraszaczy]
    L --> M[Odliczanie czasu sesji]
    M --> N[Propozycje technik relaksacyjnych]
    N --> O[Przerwa Pomodoro]

    O --> P[Statystyki i raporty]
    P --> Q{Tryb rywalizacji?}
    Q -- Tak --> R[Tryb rywalizacji]
    Q -- Nie --> S[Eksport danych / Wylogowanie]

    R --> S
    S --> T[Stop]
