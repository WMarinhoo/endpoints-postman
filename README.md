# Coleção Postman - [ServerRest API / endpoints-postman]

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![License](https://img.shields.io/github/license/[SEU-USUARIO]/[SEU-REPO]?style=for-the-badge)

> Coleção de endpoints da API **[ServerRest API]** testada e organizada no Postman. Ideal para desenvolvimento, testes manuais, automação e onboarding de novos devs.

## ✨ Visão Geral

Esta coleção contém todas as requisições principais da **[ServerRest API]**, incluindo:

- Autenticação (Login, Token, Refresh, etc.)
- Endpoints de CRUD (usuários, produtos, pedidos...)
- Requisições de busca, filtros e paginação
- Exemplos com variáveis de ambiente para diferentes ambientes (dev, staging, prod)
- Testes básicos em JavaScript (status code, tempo de resposta, schema validation)

Perfeito para quem está construindo, testando ou integrando com a API.

## 📋 Como Usar

### 1. Importar a Coleção no Postman

1. Abra o Postman (desktop ou web: https://www.postman.com)
2. Clique em **Import** (canto superior esquerdo)
3. Escolha **Link** ou **File**:
   - **Link direto** (recomendado): https://raw.githubusercontent.com/[WMarinhoo]/[endpoints-postman]/main/minha-colecao.postman_collection.json

- Ou baixe o arquivo JSON da pasta raiz e importe manualmente.
4. Após importar, configure as variáveis de ambiente (veja abaixo).

### 2. Configurar Variáveis de Ambiente

Crie um **Environment** no Postman e defina as seguintes variáveis (exemplos):

| Variável              | Exemplo (Dev)                  | Descrição                          |
|-----------------------|--------------------------------|------------------------------------|
| `baseUrl`             | `https://api.dev.suaempresa.com` | URL base da API                  |
| `apiKey` / `token`    | `seu-token-aqui`               | Chave de autenticação             |
| `userId`              | `12345`                        | ID de usuário para testes         |

Salve e selecione o environment antes de rodar as requests.

### 3. Rodar a Coleção

- Abra a coleção importada
- Use o **Collection Runner** para rodar todos os testes de uma vez
- Ou execute requests individualmente

### 4. Botão "Run in Postman" (opcional – adicione isso no README)

[![Run in Postman](https://run.pstmn.io/button.svg)](https://god.gw.postman.com/run-collection/[COLECAO-ID]?env=[ENV-ID])

*(Para gerar esse botão: publique a coleção no Postman → clique em "Share" → "Run in Postman" → copie o link e substitua aqui.)*

## 🛠 Estrutura da Coleção

Minha Coleção API
├── Autenticação
│   ├── POST Login
│   ├── POST Refresh Token
├── Usuários
│   ├── GET /users
│   ├── POST /users
│   ├── GET /users/:id
├── Produtos
│   ├── GET /products (com filtros e paginação)
│   └── ...
└── Testes Automatizados
└── Collection Runner ready


## 🚀 Dicas Úteis

- **Atualizações**: Sempre que alterar endpoints no Postman, exporte novamente (Collection → ... → Export → v2.1) e substitua o JSON no repo.
- **GitHub Actions (opcional)**: Adicione um workflow para rodar testes automáticos com Newman (CLI do Postman).
- **Documentação extra**: Use o Postman para gerar documentação automática (Publish → Documentation).

## 🤝 Contribuições

Contribuições são super bem-vindas!  
Siga estes passos:

1. Fork o repositório
2. Crie uma branch: `git checkout -b feature/nova-endpoint`
3. Commit suas mudanças: `git commit -m 'Adiciona endpoint X'`
4. Push: `git push origin feature/nova-endpoint`
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença [MIT](LICENSE) (ou a que você preferir). Veja o arquivo `LICENSE` para detalhes.

Feito com ❤️ por Wendel Marinho em Rio de Janeiro 🇧🇷  
**Última atualização:** Janeiro 2026

---

⭐ Se este repositório te ajudou, dá uma estrela para apoiar!
