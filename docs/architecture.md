````mermaid
erDiagram
    USUARIO ||--o{ POKEMON : consulta
    USUARIO ||--o{ TIME : consulta
    USUARIO ||--o{ TORNEIO : consulta
    TIME }o--|{ POKEMON : possui
    TORNEIO ||--o{ RESULTADO : possui

    USUARIO {
        int id_usuario PK
        string nome
        string email UK
        string senha
    }

    POKEMON {
        int id_pokemon PK
        string nome
        string imagem
        float percentual_uso
        string movimentos
        string habilidades
        string itens
    }

    TIME {
        int id_time PK
        string nome
        string pokemon
        float percentual_uso
    }

    TORNEIO {
        int id_torneio PK
        string nome
        date data
    }

    RESULTADO {
        int id_resultado PK
        string jogador_ou_equipe
        string colocacao
    }
```
