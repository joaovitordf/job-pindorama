# Documentação do Projeto job-pindorama

Este diretório reúne os documentos de arquitetura, guias técnicos e especificações das funcionalidades do `job-pindorama`.

## Índice de Documentos

1. [Mapa Mundial e Geolocalização de Oportunidades](MAPA_MUNDIAL_E_GEOLOCALIZACAO.md)
   - Especificação do mapa interativo (Brasil por 27 UFs e Mundo com 172 países).
   - Mecanismo de resolução geográfica e separação de modos de visualização (Volume vs Notas).
   - Otimização de renderização instantânea com `sessionStorage` e deduplicação de requisições.

2. [Integração Europeia (EURES) e Google Careers](INTEGRACAO_EURES_E_EUROPA.md)
   - Conexão oficial à base da Comissão Europeia / EURES para vagas de tecnologia.
   - Monitoramento das oportunidades de engenharia e IA no Google Careers (BH, SP e Global).
   - Modos de foco de busca (`all`, `google`, `europa`, `cv`).

3. [Arquitetura do Painel Web Local](ARQUITETURA_PAINEL.md)
   - Princípios de segurança: CSP restritivo, anti-CSRF e ausência de injeção insegura (`innerHTML`/`eval`).
   - Estrutura da API REST local (`tools/painel.py`) e componentes do frontend (`tools/painel/index.html`).
   - Fluxo de trabalho de busca, triagem em lote com IA e acompanhamento de candidaturas.

---
Para orientações de configuração e início rápido, consulte o [COMECE-AQUI.md](../COMECE-AQUI.md) e o [SETUP.md](../SETUP.md).
