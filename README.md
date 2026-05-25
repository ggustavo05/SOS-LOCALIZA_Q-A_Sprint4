# SOS Localiza — Testes de API e Qualidade

Projeto desenvolvido para validação e testes da API REST do sistema **SOS Localiza**, utilizando Azure DevOps e Insomnia.

---

# Objetivo

O objetivo desta entrega é demonstrar:

- Planejamento de testes manuais
- Criação de cenários de teste
- Validação de endpoints REST
- Configuração de autenticação Basic Auth
- Organização de testes automatizados
- Exportação de collection JSON do Insomnia

---

# Tecnologias Utilizadas

- Java Spring Boot
- Azure DevOps
- Insomnia
- Oracle Database
- Azure App Service

---

# Estrutura da Entrega

## Parte A — Testes Manuais (Azure DevOps)

Foram criados Test Cases no Azure Boards contendo:

- Nome do teste
- Objetivo
- Dados de entrada
- Passos de execução
- Resultado esperado

### Cenários Criados

- Login com credenciais válidas
- Login com senha inválida
- Login com usuário inexistente
- Login com campos vazios

---

## Azure DevOps

Adicionar aqui o link do Azure DevOps:

```txt
[Azure DevOps](https://dev.azure.com/SosLocaliza/SOS-LOCALIZA-OFC)
```

---

# Parte B — Testes Automatizados (Insomnia)

Foi utilizada uma collection do Insomnia contendo os endpoints da API REST do projeto.

## Endpoints Testados

| Método | Endpoint |
|--------|-----------|
| GET | /actuator/health |
| GET | /api/eventos/ativos |
| GET | /api/mobile/me |
| GET | /api/sms/getAll |

---

# Autenticação

A API utiliza autenticação:

```txt
Basic Auth
```

## Usuário USER

```txt
citizen
password
```

## Usuário ADMIN

```txt
admin
password
```

---

# Collection Insomnia

O arquivo:

```txt
SOS_Localiza.insomnia.json
```

contém:

- Endpoints da API
- Configuração de autenticação
- Requests organizadas
- Configurações de ambiente

---

# Como Importar a Collection

1. Abrir o Insomnia
2. Clique em:
   ```txt
   Import
   ```
3. Selecionar o arquivo:
   ```txt
   SOS_Localiza.insomnia.json
   ```

---

# Ambientes da API

## Produção

```txt
https://soslocaliza-api-prod-560242.azurewebsites.net
```

## Staging

```txt
https://soslocaliza-api-staging-560242.azurewebsites.net
```

---

# Estrutura do Projeto

```txt
README.md
SOS_Localiza.insomnia.json
```

---

# Integrantes

- Gustavo Gonçalves

---

# Observações

Os testes foram realizados utilizando autenticação Basic Auth e endpoints disponibilizados pela API do projeto SOS Localiza.

A collection exportada em JSON permite reproduzir os testes diretamente no Insomnia.
