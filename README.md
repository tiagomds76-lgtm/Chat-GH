# Chat-GH

Repositório central para organizar vários tipos de software em construção.

A ideia deste repositório é funcionar como uma base limpa, segura e preparada para receber projetos diferentes: sistemas web, aplicativos, automações, scripts, integrações com IA, banco de dados, documentação técnica e estudos de arquitetura.

> Importante: este repositório está público. Não coloque dados sigilosos, senhas, tokens, chaves de API, documentos internos de cliente, certificados, cookies, arquivos `.env` reais ou informações estratégicas que não possam aparecer na internet.

---

## Estrutura geral recomendada

```text
Chat-GH/
├── apps/
│   ├── web/                    # Sistemas web, painéis, dashboards
│   ├── mobile/                 # Aplicativos Android/iOS
│   ├── desktop/                # Programas para computador
│   └── api/                    # APIs principais
├── packages/
│   ├── ui/                     # Componentes visuais reutilizáveis
│   ├── core/                   # Regras de negócio compartilhadas
│   └── utils/                  # Funções auxiliares
├── backend/
│   ├── src/                    # Código do servidor
│   ├── tests/                  # Testes do backend
│   └── docs/                   # Documentação técnica do backend
├── frontend/
│   ├── src/                    # Código da interface
│   ├── public/                 # Arquivos públicos
│   └── tests/                  # Testes do frontend
├── banco-de-dados/
│   ├── migrations/             # Alterações estruturais do banco
│   ├── seeds/                  # Dados iniciais de teste
│   ├── diagramas/              # Modelos e DER
│   └── consultas/              # Queries SQL úteis
├── automacoes/
│   ├── scripts/                # Robôs, tarefas repetitivas e utilitários
│   ├── agentes-ia/             # Prompts, agentes e fluxos com IA
│   └── monitoramentos/         # Alertas, verificadores e rotinas
├── integracoes/
│   ├── apis-externas/          # Integrações com sistemas de terceiros
│   ├── webhooks/               # Recebimento/envio de eventos
│   └── modelos/                # Exemplos de payloads e contratos
├── infraestrutura/
│   ├── docker/                 # Dockerfiles e docker-compose
│   ├── deploy/                 # Publicação em servidor/nuvem
│   ├── github-actions/         # CI/CD e automações do GitHub
│   └── ambientes/              # dev, homologação e produção
├── documentos/
│   ├── requisitos/             # O que o sistema precisa fazer
│   ├── propostas/              # Propostas comerciais/técnicas
│   ├── atas-reunioes/          # Decisões e alinhamentos
│   ├── manuais/                # Como usar o sistema
│   └── pesquisas/              # Estudos, referências e comparativos
├── planejamento/
│   ├── roadmap/                # Etapas do projeto
│   ├── tarefas/                # Lista de tarefas e prioridades
│   ├── arquitetura/            # Decisões técnicas importantes
│   └── ideias/                 # Ideias futuras sem compromisso imediato
├── testes-gerais/              # Testes de conceito e experimentos
├── .github/
│   ├── ISSUE_TEMPLATE/         # Modelos de tarefas, bugs e melhorias
│   └── workflows/              # Automações do GitHub Actions
├── .gitignore
├── .env.example
├── CONTRIBUTING.md
├── SECURITY.md
└── README.md
```

---

## Para que serve cada área

| Área | Uso principal |
|---|---|
| `apps/` | Projetos finais: web, mobile, desktop e APIs |
| `packages/` | Partes reaproveitáveis entre vários softwares |
| `backend/` | Servidor, regras de negócio, autenticação e integrações |
| `frontend/` | Telas, painéis, formulários e experiência do usuário |
| `banco-de-dados/` | Estrutura, consultas, migrations, seeds e diagramas |
| `automacoes/` | Robôs, scripts, agentes de IA e monitoramentos |
| `integracoes/` | APIs externas, webhooks e formatos de comunicação |
| `infraestrutura/` | Docker, deploy, ambientes e automações de publicação |
| `documentos/` | Requisitos, manuais, propostas, atas e pesquisas |
| `planejamento/` | Roadmap, tarefas, arquitetura e ideias futuras |
| `testes-gerais/` | Experimentos sem comprometer o projeto principal |

---

## Tipos de software que esta base suporta

### 1. Sistema web
Exemplo: painel para acompanhar pregões, propostas, documentos e alertas.

### 2. Aplicativo mobile
Exemplo: app para receber notificações de chamadas do pregoeiro.

### 3. Software desktop
Exemplo: programa instalado no Windows para monitorar várias abas, arquivos e alertas locais.

### 4. API/backend
Exemplo: servidor que centraliza dados, usuários, permissões e integrações externas.

### 5. Robôs e automações
Exemplo: scripts que verificam sites, e-mails, planilhas ou portais e geram alertas.

### 6. Agentes de IA
Exemplo: agentes que leem mensagens, classificam urgência, resumem editais e sugerem respostas.

### 7. Banco de dados
Exemplo: tabelas de pregões, UASGs, órgãos, fornecedores, produtos, lances, documentos e prazos.

### 8. Documentação e planejamento
Exemplo: requisitos, mapa do sistema, decisões técnicas, manuais e roteiro de desenvolvimento.

---

## Regras básicas de segurança

Nunca subir para o GitHub:

```text
senhas reais
chaves de API
tokens
certificados
arquivos .env reais
cookies de navegador
dados pessoais sensíveis
contratos sigilosos
documentos internos de cliente
prints com informações privadas
```

Use sempre arquivos de exemplo:

```text
.env.example
config.example.json
credentials.example.json
```

---

## Fluxo de trabalho recomendado

1. Criar uma tarefa em `planejamento/tarefas/` ou nas Issues do GitHub.
2. Descrever claramente o objetivo.
3. Criar ou editar arquivos na pasta correta.
4. Testar localmente ou no Codespaces.
5. Fazer commit com mensagem clara.
6. Revisar antes de colocar dados reais.

Exemplo de mensagem de commit:

```text
Adicionar estrutura inicial para monitoramento de pregões
```

---

## Próximos arquivos úteis

Esta base deve receber:

```text
.gitignore
.env.example
CONTRIBUTING.md
SECURITY.md
.github/ISSUE_TEMPLATE/bug_report.md
.github/ISSUE_TEMPLATE/feature_request.md
.github/ISSUE_TEMPLATE/tarefa.md
.github/workflows/ci.yml
```

---

## Observação final

Esta estrutura é ampla de propósito. Ela evita que o projeto nasça bagunçado e permite receber vários softwares diferentes sem precisar reorganizar tudo depois.

Para projeto sério, comercial ou com dados estratégicos, o ideal é usar repositório privado.
