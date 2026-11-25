# UpGrade

Sistema de metabusca online que compara preços e ofertas de hardware em vários sites ao mesmo tempo, mostrando ao usuário os melhores preços, frete, prazo de entrega e a qualificação das lojas.

Projeto Integrador Extensionista II (PIE II) · Análise e Desenvolvimento de Sistemas.

## Status do projeto

Esqueleto inicial (Atividade 1): front-end com Vite+ e API Express com a rota de verificação `GET /api/health`, exibida na página inicial.

## Tecnologias

- Vite+ (front-end, JavaScript Vanilla)
- Node.js e Express (API)
- dotenv (variáveis de ambiente)

## Requisitos

- Git
- Node.js 20 ou superior
- Vite+ (comando `vp`): https://viteplus.dev

## Como rodar

1. Clone o repositório e entre na pasta:

   ```bash
   git clone https://github.com/0FerreiraDevJr/ads-pie2-upgrade.git
   cd ads-pie2-upgrade
   ```

2. Instale as dependências:

   ```bash
   vp install
   ```

3. Crie o arquivo de variáveis de ambiente a partir do exemplo:

   ```bash
   cp .env.example .env
   ```

   No Windows (PowerShell): `copy .env.example .env`

4. Em um terminal, inicie a API:

   ```bash
   vp run api
   ```

5. Em outro terminal, inicie o front-end:

   ```bash
   vp dev
   ```

6. Abra http://localhost:5173 no navegador. A página deve mostrar **"Status da API: ok"** com data e hora.

## Rotas da API

| Método | Rota          | Descrição                             |
| ------ | ------------- | ------------------------------------- |
| GET    | `/api/health` | Retorna o status da API e a data/hora |

## Estrutura

```
├── server/
│   └── index.js        # API Express
├── index.html
├── main.js             # Página inicial (consome /api/health)
├── vite.config.ts      # Configuração do Vite+ e proxy /api
├── .env.example        # Modelo das variáveis de ambiente
└── package.json
```

## Autor

Seu Nome · [GitHub](https://github.com/0FerreiraDevJr)
