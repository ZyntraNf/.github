# Zyntra

<p align="center">
  <img width="1536" height="1024" alt="ChatGPT Image May 7, 2026, 11_45_01 PM (1)" src="https://github.com/user-attachments/assets/98b33997-2710-4fe1-b8c4-36a14c49e8be" />
</p>

<p align="center">
  Sistema moderno para emissão e gerenciamento de documentos fiscais eletrônicos.
</p>

---

## Sobre

O Zyntra é uma plataforma focada em emissão fiscal, desenvolvida para centralizar e simplificar integrações com a SEFAZ.

O projeto foi criado com foco em:

- Organização
- Escalabilidade
- Performance
- Segurança
- Arquitetura modular

---

# Arquitetura

O projeto segue uma arquitetura modular baseada em domínio.

```txt
src/
├── common/
│
├── config/
│
├── modules/
│   ├── auth/
│   │
│   ├── companies/
│   │
│   ├── customers/
│   │
│   ├── certificates/
│   │
│   ├── payments/
│   │
│   └── invoices/
│       ├── nfcom/
│       └── nfe/
│
│
└── main.ts
```

---

# Stack

## Backend

- Node.js
- NestJS
- TypeScript

## Banco de Dados

- PostgreSQL
- Prisma ORM

## Fiscal

- XML Builder
- XML Signature
- Certificado A1
- Integração SEFAZ

---

# Funcionalidades

## Autenticação

- JWT
- Controle de acesso
- Refresh Token

## Empresas

- Cadastro de emitentes
- Configuração fiscal
- Upload de certificados

## Clientes

- Gestão de clientes
- Dados fiscais
- Histórico

## Emissão Fiscal

- Emissão de NFCom
- Geração de XML
- Assinatura digital
- Envio para SEFAZ
- Consulta de status
- Eventos fiscais

## PDF

- Geração de DANFE
- Download de PDF

---

# Estrutura do Projeto

Cada módulo possui:

```txt
module/
├── controllers/
├── services/
├── dto/
├── entities/
├── repositories/
└── module.ts
```

---

# Fluxo da Emissão

```txt
Pagamento aprovado
        ↓
Validação fiscal
        ↓
Geração XML
        ↓
Assinatura digital
        ↓
Envio SEFAZ
        ↓
Autorização
        ↓
Geração DANFE/PDF
        ↓
Persistência no banco
```

---

# Objetivos

O Zyntra foi desenvolvido para:

- Centralizar operações fiscais
- Reduzir complexidade de integração
- Facilitar manutenção
- Permitir crescimento modular
- Suportar novos documentos fiscais futuramente

---

# Roadmap

## MVP

- [x] Estrutura inicial
- [ ] Autenticação
- [ ] Cadastro de empresas
- [ ] Upload de certificados
- [ ] Emissão NFCom
- [ ] Geração XML
- [ ] Integração SEFAZ
- [ ] Geração DANFE

## Futuro

- [ ] NF-e
- [ ] NFC-e
- [ ] CT-e
- [ ] Dashboard administrativo
- [ ] Multiempresa
- [ ] Webhooks

---

# Status

🚧 Em desenvolvimento

---

# Licença

Privado — Todos os direitos reservados.

---
