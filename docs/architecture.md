# 🛠️ Especificação Técnica (Tech Spec) - Watchlog

Este documento detalha a arquitetura técnica, o modelo de dados e os contratos de API (via JSON Server) necessários para o funcionamento do sistema Watchlog.

## 1. Modelo de Dados (Diagrama ER)

Abaixo está o Diagrama Entidade-Relacionamento (DER) que representa a estrutura do nosso "banco de dados" (`db.json`) e como as informações se conectam.

```mermaid
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

## 2. Tecnologias Utilizadas

Abaixo terão as especificações tecnicas do que será utilizado no projeto.

- **Bootstrap** - v5.3
- **JQuey** - v4.0.0
- **JSON Server** - v1.0.0
- **Pokemon Champions Battle Data API** - v1.0
- **PokéApi** - v2.0
