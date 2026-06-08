# 🥚 BrStorm — Controle e Automação de Granja

> *A viagem — criatório de aves ornamentais e melhoramento de poedeiras*

**Status:** 🟢 Live  
**URL:** [agilitybrstorm.github.io/Brstorm](https://agilitybrstorm.github.io/Brstorm/)  
**Última atualização:** 08/06/2026

---

## Sobre o projeto

BrStorm é uma aplicação web para controle e automação completa de granja, desenvolvida para uso interno da criação de aves ornamentais e poedeiras da marca BrStorm.

O projeto é construído de forma incremental — um módulo por vez — com foco em visualização de dados, usabilidade mobile e acesso multiusuário em tempo real.

---

## Status atual — v5

**Módulo ativo:** Controle de Incubação

Funcionalidades implementadas:
- Bandeja de incubação com 63 posições (7 colunas × 9 linhas)
- Cadastro de ovos por posição com nome do cruzamento
- Contagem automática de posições ocupadas e livres
- Tempo decorrido de incubação por posição (dias e horas)
- Relógio em tempo real com fuso horário de São Paulo
- Autenticação com dois níveis de acesso: Admin e Visualizador
- Dados sincronizados em nuvem via Supabase
- Acesso via qualquer dispositivo e navegador

---

## Stack técnica

| Componente | Tecnologia |
|---|---|
| Frontend | HTML + CSS + JavaScript (arquivo único) |
| Hospedagem | GitHub Pages (gratuito) |
| Banco de dados | Supabase (PostgreSQL) |
| Autenticação | Supabase Auth |
| Repositório | GitHub |

---

## Acesso

**URL pública:** https://agilitybrstorm.github.io/Brstorm/

O acesso requer login com e-mail e senha. Dois níveis de permissão:
- **Admin** — visualiza e edita todos os registros
- **Visualizador** — somente leitura

Credenciais gerenciadas pelo administrador via Supabase.

---

## EVOLUÇÃO DO APP 

- estrutura do app
	- utilização do claude code
	- hospedagem com url própria
	- Separação dos módulos 
	- Landing page com pré-visualização de todos os módulos

- Próximos módulos planejados
- Modulo Controle de Incubação
	- Histórico de incubações e eclosões
	- Resultado de ovoscopias
	- Controle de temperatura e umidade centralizado

- poedeiras
	- Taxa de conversão alimentar por lote
	- Controle de lotes de poedeiras (alimentação, produção, custo)

- ornamentais
	- Controle individual de baías (recria e ornamentais)

- controle via app da automação total da granja
	- Automação com Arduino e ESP32
	- alimentador
	- controle de ingestão de agua
	- tratamento e classificação dos ovos
	- tags para melhoramento individual e controle de otimização de lotes

---

## Histórico de versões

| Versão | Data | Descrição |
|---|---|---|
| v1 | 04/06/2026 | Versão inicial — bandeja local com localStorage |
| v2 | 04/06/2026 | Upload inicial no GitHub Pages |
| v3 | 08/06/2026 | Correções visuais: grid fixo, 4 infos no ovo, fundo verde oliva |
| v4 | 08/06/2026 | Integração Supabase — autenticação e tabela user_roles |
| v5 | 08/06/2026 | Correção fuso horário no timestamp de incubação |

---

## Processo de atualização

1. Baixar `index.html` atual do repositório
2. Realizar alterações com auxílio de IA (Claude)
3. Subir via **Carregar arquivo** no repositório GitHub
4. Confirmar na URL pública
