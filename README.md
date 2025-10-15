# Sistema de Gestão de Ótica

Sistema completo para gestão de óticas com funcionalidades de cadastro de clientes, vendas, controle de pagamentos e impressão de recibos.

## Funcionalidades

- **Autenticação**: Sistema de login seguro
- **Gestão de Clientes**: Cadastro completo com prescrições oftálmicas
- **Vendas**: Registro de vendas com controle de pagamentos
- **Recibos**: Impressão de recibos com informações da loja e prescrição
- **Dashboard**: Visão geral das vendas e estatísticas
- **Perfil da Empresa**: Configuração dos dados da ótica

## Tecnologias

### Web App
- **Frontend**: React + TypeScript + Vite
- **Backend**: Convex (banco de dados reativo)
- **Estilização**: TailwindCSS
- **Autenticação**: Convex Auth

### Android App
- **Linguagem**: Kotlin
- **WebView**: Para exibir o app web
- **Compatibilidade**: Android 7.0+ (API 24+)

## Instalação

### Web App

1. Clone o repositório
2. Instale as dependências:
   ```bash
   npm install
   ```
3. Configure o Convex:
   ```bash
   npx convex dev
   ```
4. Inicie o servidor de desenvolvimento:
   ```bash
   npm run dev
   ```

### Android App

1. Abra o Android Studio
2. Importe o projeto da pasta `android/`
3. Atualize a URL do app em `MainActivity.kt`:
   ```kotlin
   private val APP_URL = "https://sua-url-do-convex.com"
   ```
4. Execute o projeto no dispositivo ou emulador

## Estrutura do Projeto

```
/
├── src/                    # Código fonte React
├── convex/                 # Backend Convex
├── android/                # App Android
├── public/                 # Arquivos públicos
└── README.md
```

## Configuração do Recibo

O sistema gera recibos com:
- Informações da loja (nome fantasia, CNPJ, telefone)
- Dados do cliente e prescrição oftálmica
- Itens vendidos (armação, lentes, acessórios)
- Valores e forma de pagamento
- Data prevista para entrega
- Termos de garantia

## Desenvolvimento

Para contribuir com o projeto:

1. Faça um fork do repositório
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Abra um Pull Request

## Licença

Este projeto está sob a licença MIT.
