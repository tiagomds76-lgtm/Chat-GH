# Como contribuir e organizar o trabalho

Este repositório serve para receber vários tipos de software. Para manter tudo organizado, siga este padrão.

## Antes de começar uma tarefa

1. Descreva o objetivo.
2. Identifique qual área será alterada.
3. Evite misturar muitos assuntos no mesmo commit.
4. Confira se nenhum dado sensível foi incluído.

## Padrão de commits

Use mensagens simples e claras:

```text
Adicionar estrutura inicial do backend
Criar documentação do banco de dados
Corrigir validação de formulário
Adicionar script de monitoramento
```

## Organização por tipo de projeto

- Sistemas web: `apps/web/` ou `frontend/`
- APIs: `apps/api/` ou `backend/`
- Mobile: `apps/mobile/`
- Desktop: `apps/desktop/`
- Automações: `automacoes/`
- Integrações: `integracoes/`
- Banco de dados: `banco-de-dados/`
- Documentos e planejamento: `documentos/` e `planejamento/`

## Revisão antes de subir código

Antes de fazer commit, confira:

- O código roda?
- O arquivo está na pasta certa?
- Tem senha, token ou chave exposta?
- O nome do arquivo está claro?
- A alteração tem relação com a tarefa?
