# BugHunter

Produto real da DouglasDev para operacao de bugs com painel interativo full stack.

## O que este repositorio entrega
- API Node/Express com validacao de entrada via Zod.
- Persistencia local de dados em arquivo (modo desenvolvimento/producao).
- Filtros reais por status, prioridade e busca textual.
- Exportacao CSV para analise operacional.
- Frontend React responsivo com feedback de carregamento/erro e interacoes completas.

## Fluxo operacional
1. Receber bug e registrar contexto minimo obrigatorio.
2. Classificar impacto e definir prioridade da correcao.
3. Executar ajuste, validar e marcar como concluido.

## Endpoints principais
- `GET /health`
- `GET /api/meta`
- `GET /api/work-items`
- `GET /api/work-items/export.csv`
- `POST /api/work-items`
- `PATCH /api/work-items/:id/toggle`
- `DELETE /api/work-items/:id`

## Setup
1. `npm install --include=dev`
2. `npm run bootstrap`
3. `npm run dev`

## Qualidade
- `npm run quality` executa lint + testes + build no backend e frontend.

## Marca
DouglasDev
