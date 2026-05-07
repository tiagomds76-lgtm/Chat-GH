# Segurança

Este repositório pode receber diferentes tipos de software. Por isso, algumas regras são obrigatórias.

## Nunca enviar para o GitHub

- Senhas reais
- Tokens
- Chaves de API
- Certificados
- Arquivos `.env` reais
- Cookies
- Dados pessoais sensíveis
- Contratos sigilosos
- Documentos internos de clientes
- Prints com informações privadas

## Como trabalhar com segurança

Use arquivos de exemplo, como:

```text
.env.example
config.example.json
credentials.example.json
```

Os valores reais devem ficar apenas no computador local, servidor, GitHub Secrets ou ambiente seguro.

## Em caso de vazamento

1. Remova imediatamente o arquivo ou segredo.
2. Revogue a chave/token no serviço original.
3. Gere uma nova chave.
4. Revise o histórico do repositório se necessário.
