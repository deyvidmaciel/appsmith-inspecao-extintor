# 🧯 Sistema de Inspeção de Extintores (Appsmith SaaS)

Este projeto é um *sistema de gestão de inspeção de extintores* desenvolvido em *[Appsmith](https://appsmith.com)* no modelo *SaaS*.  
O sistema permite cadastro de extintores, geração de QR Codes, registro de inspeções e emissão de relatórios.

---

## 🚀 Funcionalidades

- Login seguro (com hash de senha no banco).
- Cadastro de clientes (multi-tenant SaaS).
- Cadastro e gerenciamento de extintores.
- Geração automática de *QR Code* para cada extintor.
- Registro de inspeções com status e observações.
- Relatórios exportáveis (CSV/Excel).
- Suporte a múltiplos clientes no mesmo banco (*multi-tenant*).

---

## 🗄 Banco de Dados

Este projeto suporta *Postgres* ou *MySQL*.  

### Estrutura das tabelas principais
- *Clientes* → empresas que utilizam o sistema.  
- *Usuarios* → usuários vinculados a cada cliente.  
- *Extintores* → cadastro dos equipamentos.  
- *Inspecoes* → histórico de inspeções.  

> Script SQL completo disponível em: docs/database.sql

---

## 🔑 Segurança

- As senhas são salvas com *hash (bcrypt/pgcrypto)*.  
- Nunca armazene senha em texto puro.  
- Recomenda-se configurar variáveis de ambiente (.env ou secrets.env) para credenciais do banco.

---

## 📥 Importar no Appsmith

1. Acesse seu *Appsmith Cloud* ou instância própria (Docker).  
2. Clique em *Create New → Import App*.  
3. Carregue o arquivo:  
4.
