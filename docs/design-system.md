🎨 Design System — Watchlog (Competitive Analytics VGC)

Neste projeto, desenvolvemos uma interface analítica voltada para competidores de alto nível de Pokémon Champions (VGC Doubles), combinando a estética de telemetria esports com o rigor analítico de dados em tempo real.



1. Framework Base & Arquitetura Visual





Framework Escolhido: Bootstrap 5 (Customizado via Sass / Variáveis CSS nativas)



Motivação: Proporciona um sistema de grid robusto de 12 colunas (container-fluid, row, col-*), componentes padronizados prontos para produção (Navbar, Cards, Badges, Modals, Progress bars) e flexibilidade completa para sobrescrever variáveis de tema via classes utilitárias e regras Sass, permitindo um visual Dark Esports profissional sem abrir mão da consistência e facilidade de manutenção do Bootstrap.



2. Paleta de Cores (Customização de Variáveis)

As variáveis de cor foram integradas ao tema customizado do Bootstrap ($theme-colors) para oferecer contraste cirúrgico em monitores e telas mobile sob iluminação de arena ou ambientes escuros:





Cor Primária ($primary / Ação & Telemetria Ativa): #06B6D4 (Cyan / Electric Cyan)





Uso: Botões principais (.btn-primary), indicadores de telemetria em tempo real (LIVE S3), barras de progresso (.progress-bar.bg-primary) e foco em inputs de busca. Simboliza precisão tecnológica e agilidade esportiva.



Hover / Foco: #0891B2 (Cyan 600) para feedback tátil imediato.



Cor Secundária ($secondary / Tática & Estratégia): #3B82F6 (Royal Tactical Blue)





Uso: Badges táticos (.badge.bg-secondary), links secundários, filtros avançados e marcadores de chaveamento.



Cor de Fundo (Canvas Global / $body-bg): #0F131D (Dark Esports Slate)





Uso: Fundo padrão de todas as páginas da aplicação para reduzir a fadiga visual durante longas sessões de análise competitiva.



Superfícies & Containers ($card-bg / Painéis Elevados): #131824 e #171B26





Uso: Superfícies elevadas para cards de Pokémon (.card), esquadrões de torneio e painéis laterais de sinergia, delimitados por bordas translúcidas sutis (border: 1px solid rgba(255, 255, 255, 0.08)).



Cores Semânticas de Performance & Status:





Sucesso / Winrate Positiva ($success): #10B981 (Emerald 500) — Taxas de vitória superiores a 50%, partidas vitoriosas e status de conexão online.



Aviso / Meta Leader #1 ($warning): #F59E0B (Amber 500) — Badges de campeão invicto, Rank #1 e avisos táticos de meta.



Perigo / Fraqueza Crítica ($danger): #EF4444 (Red 500) — Matriz de counters, fraquezas 4x a gelo/fada e alertas de ameaça em campo.



Informativo / Tags de Torneio ($info): #38BDF8 (Sky Blue) — Marcadores de rodadas, tags M-B e metadados informativos.



Tipagens Oficiais de Batalha (18 Tipos VGC):





Cores utilitárias de alto contraste para badges de tipos (Dragão #4F46E5, Terrestre #B45309, Grama #15803D, Fantasma #6B21A8, Água #0284C7, Fogo #EA580C, Aço #475569, Fada #DB2777).



3. Tipografia

Importada via Google Fonts para criar uma divisão funcional rigorosa entre leitura geral e telemetria numérica:





Títulos (H1 a H6), Navegação e Rótulos Gerais: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif (Pesos: 500 Medium, 600 SemiBold, 700 Bold).





Motivação: Proporciona legibilidade cristalina em interfaces escuras densas, com kerning otimizado para telas de alta densidade de pixels.



Métricas Numéricas, Rental Codes & Spreads: JetBrains Mono / Roboto Mono, monospace (Pesos: 500 Medium, 700 Bold).





Motivação: Garante alinhamento tabular perfeito para porcentagens (48.05%), somatórios de atributos de Pokémon e limite regulamentar de 66 EVs máximos do Champions.



4. Diretrizes de Uso de Componentes

Regras de aplicação dos componentes do Bootstrap dentro da lógica analítica e competitiva do Watchlog:





Botões de Ação (.btn):





Ações de alta prioridade de fluxo (Cadastre-se Gratuitamente, Exportar Showdown, Copiar Rental Code) usam .btn.btn-primary com texto escuro invertido (color: #0A0E18; font-weight: 600; border-radius: 8px).



Ações analíticas secundárias ou de filtro usam visual outline escuro (.btn.btn-outline-secondary ou custom .btn-outline-cyan) com borda translúcida e hover suave.



Cards Analíticos & Esquadrões (.card):





Cards de equipes e fichas técnicas de Pokémon utilizam background elevado (.card com fundo #171B26), borda translúcida (border-color: rgba(255, 255, 255, 0.08)) e espaçamento padronizado (.card-body.p-3.p-lg-4).



O Pokémon Rank #1 do metagame (Garchomp) recebe contorno de destaque sutil em tom dourado/âmbar ou ciano com a tag .badge.bg-warning (#1 META LEADER).



Tabelas de Metagame (.table):





Tabelas analíticas utilizam as classes .table.table-dark.table-hover com divisores sutis de borda, alinhamento vertical centralizado (.align-middle) e barras de progresso horizontais (.progress com .progress-bar.bg-primary) para indicar o percentual de uso.



Badges & Tags de Identificação (.badge):





Utilizadas para tipagens elementais, formatos de torneio e posições no ranking. Usam cantos arredondados suaves (.rounded-pill ou rounded-1) com padding equilibrado para exibição compacta.



Spreads de EVs e Regras do Regulamento:





Toda ficha técnica de Pokémon deve respeitar a soma limite de 66 EVs (padrão oficial Champions Reg M-B), destacando o arquétipo de velocidade (+Spe) e dano em fontes monoespaçadas.
