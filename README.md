# Nexo Cirúrgico — v1.4.4 (auditoria curricular)

Plataforma de treinamento de procedimentos médicos e cirúrgicos voltada a estudantes e médicos em treinamento supervisionado.

## Atualização de leitura

Aulas e fichas práticas exibem textos em 18 px por padrão, com controle de tamanho de 16 a 22 px. Implementado seletor PT/ES **beta para a interface**. **O conteúdo clínico das 115 aulas e 46 fichas permanece em português**, aguardando tradução médica revisada.

## Auditoria de cinco manuais

A matriz curricular foi confrontada com cinco livros fornecidos pelo responsável editorial. Resultado: 46 fichas em 227 tópicos, 21 módulos sem fichas, incluindo M16 Cirurgia Geral. O documento original de auditoria está dentro de `project-source.tar.gz` em `AUDITORIA_CINCO_MANUAIS_CURRICULO_2026-10-15.md`. Os PDFs e imagens protegidas por direitos autorais NÃO integram este repositório.

## Build

`tar -xzf project-source.tar.gz && npm run build && npm run qa:deploy` — publica somente a pasta `dist`. Os testes automáticos devem incluir `npm run qa`, `npm run qa:typography` e `npm run qa:reader-lang`.

**Não é protocolo assistencial validado.** É necessária revisão médica, simulação e supervisão. Product by InMed.
