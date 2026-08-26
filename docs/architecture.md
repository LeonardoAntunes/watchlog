flowchart TD
    Login["LOGIN"] -->|Autenticação| Aplicacao["APLICAÇÃO"]

    Aplicacao --> Pokemon["Pokémon no Meta"]
    Aplicacao --> Times["Times no Meta"]
    Aplicacao --> Torneios["Resultados de Torneios"]

    Pokemon --> Detalhes["Detalhes do Pokémon"]

    classDef auth fill:#fef2f2,stroke:#f87171,stroke-width:2px
    classDef app fill:#eef2ff,stroke:#818cf8,stroke-width:2px
    classDef feature fill:#f0fdfa,stroke:#2dd4bf,stroke-width:1.5px
    classDef detail fill:#fff7ed,stroke:#fb923c,stroke-width:1.5px

    class Login auth
    class Aplicacao app
    class Pokemon,Times,Torneios feature
    class Detalhes detail
