# Sistema de Ferias e Licenca Premio

Aplicacao web para o controle de ferias e licenca premio da equipe de Radiologia.

## Recursos

- Cadastro de membros da equipe.
- Lancamentos de ferias e licenca premio.
- Filtros de consulta por servidor, beneficio e periodo.
- Exportacao de membros e lancamentos em XML.
- Persistencia local no navegador com IndexedDB e fallback em localStorage.
- Suporte a instalacao como PWA.

## Execucao local

Abra `index.html` em um navegador para utilizar a aplicacao. Para testar a instalacao PWA e o cache offline, hospede os arquivos por HTTP local ou HTTPS.

## Persistencia de dados

Os dados ficam armazenados somente no navegador e no dispositivo em uso. A limpeza dos dados do navegador remove esses registros. Antes da publicacao em producao, os dados devem ser migrados para um backend com banco de dados, controle de acesso e backups.

## Arquivos principais

- `index.html`: interface, regras de negocio, armazenamento local e geracao de XML.
- `manifest.json`: metadados da aplicacao instalavel.
- `service-worker.js`: cache offline do PWA.
