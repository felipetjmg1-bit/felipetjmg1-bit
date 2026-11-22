# Plano de execução técnica do portfólio Impulso Digital

**Atualizado em:** 22/11/2026  
**Escopo observado:** 34 repositórios públicos da conta `felipetjmg1-bit`.  
**Status desta revisão:** inventário de READMEs e inspeção direcionada de código/dependências em projetos prioritários. Não equivale a execução integral dos builds, testes ou auditoria linha a linha de todos os repositórios.

## Objetivo

Preparar cada repositório para avaliação técnica por universidades, parceiros, patrocinadores e investidores, preservando o histórico e o código original. Nenhum projeto recebe status de produção, homologado, validado externamente ou 100% concluído sem evidência verificável.

## Regra de classificação

- **Implementação em validação:** existe código executável, mas ainda requer validação, testes ou controles de segurança.
- **Demonstração:** interface, fluxo simulado ou integração parcial. Dados e funções simuladas devem estar identificados.
- **Pesquisa/proposta:** hipótese, whitepaper ou arquitetura ainda sem implementação operacional.
- **Fork/infraestrutura:** código derivado ou ferramenta auxiliar; atribuição e licença precisam estar claras.

## Ordem de engenharia

### P0: demonstradores prioritários

1. **aurora-geointelligence-xai** — validar instalação limpa, dependências, GeoTIFF/CRS/NoData, limites de upload e suíte de testes; publicar demo e resultados reproduzíveis. O agrupamento MiniBatchKMeans é visual e não semântico; não alegar classificação de cobertura do solo ou XAI de modelo supervisionado.
2. **sentinela-brasil** — revisar autenticação/autorização por rota, bootstrap, rotação e backup de chaves, criptografia, ledger, upload, privacidade e testes de integração/abuso. API local com testes automatizados aprovados; ainda não é implantação de produção.
3. **oraculo-x37** — reconciliar Flask/FastAPI, versões de dependências, imports, execução do MCP, modelos serializados, configuração DEBUG e exposição de rede. Adicionar CI e documentação de deploy.
4. **Can-rio-amarelo- / canario-amarelo-versao-soberana / ORACULOX37-V-3.6.9** — separar funções Speckle Automate de serviços ML/MCP; confirmar o módulo `flatten.flatten_base`; criar fixtures BIM e testes heurísticos. Não alegar certificação normativa ou cálculo estrutural.

### P1: pesquisa com software/simulação

5. **projeto-ybyra** — converter workflow de template em CI somente após confirmar os comandos de instalação e teste; identificar claramente dados sintéticos e simulações.
6. **sentinela-das-aguas-app** — validar frontend, API, schema/migrações, autenticação, autorização e origem dos dados. O repositório sentinela-das-aguas permanece proposta até existir pipeline operacional.
7. **aurora-xai-2-5, App-impulso-digital-, aurora-kids-alfa, Chat-gpt-aurora-, CRISTAL-5D-V.4.0-MODULO-1** — distinguir dados mock de integrações reais; validar configuração, privacidade, erros, custos e segurança.
8. **cristal-quartzo-aurora, ucu-crystal-control-unit-v2, aurora-omni-kernel, Aurora-Sovereign-Intelligence, EVA-IA** — completar contratos, dependências, persistência, testes e documentação; manter claims de hardware/integrações como pesquisa até validação.

### P2: propostas e conceitos

9. **SQO-Supercomputador-Quantico-Orbital, quartz-5d-sovereignty, ucu-crystal-control-unit, Terrabras, sentinela-das-aguas, aurora-soberana, canario-soberano-x, Provas-de-Conceito-IA** — publicar hipótese, problema, estado atual, TRL estimado com justificativa, requisitos, riscos, fontes, orçamento por cotação e protocolo de validação. Não descrever proposta como produto operacional.

### P3: vitrine, forks e ativos auxiliares

10. **aurorashop-page-app, felipetjmj1.github.io, portfolio-template, Mobile-Console-Viewer, ton-assets, SENTINELA-SOBERANO-2037** — declarar escopo real, revisar licença/origem, identificar simulações e proteger dados. Base64 não é criptografia. Forks devem manter upstream e atribuição.

## Padrão de conclusão para software

Cada software deve possuir, conforme sua stack:
- README com problema, público, estado, recursos existentes, limitações, arquitetura, requisitos, instalação, execução e exemplos;
- licença válida e inventário de ativos/terceiros;
- manifesto e lockfile reproduzíveis;
- `.env.example` sem segredos;
- testes unitários, integração e regressão;
- CI em push e pull request com lint, testes e build;
- `SECURITY.md`, `CONTRIBUTING.md`, changelog e política de suporte;
- Dependabot e controles de segredos/dependências quando disponíveis;
- release versionada, demo reproduzível e evidência de execução;
- para modelos/dados: model card/dataset card com origem, licença, métricas, limites e avaliação;
- para software distribuído: SBOM e processo de atualização de dependências.

Projetos documentais e de pesquisa não devem receber CI de software artificial. Devem ter revisão editorial/científica, rastreabilidade de fontes, protocolo e entregáveis de pesquisa.

## Critérios de aceite

Um projeto recebe o selo interno **Vitrine verificada** somente quando:
1. instalação limpa documentada e reproduzida;
2. execução principal confirmada;
3. testes/build aprovados em CI;
4. dependências e segurança revisadas;
5. licença e proveniência verificadas;
6. demo coerente com o código;
7. arquitetura, limites e riscos documentados;
8. release versionada;
9. nenhum segredo/dado pessoal exposto;
10. evidência técnica arquivada.

O selo é interno e não representa certificação, homologação ou validação independente.

## Limites desta execução

O conector GitHub permite ler e gravar arquivos e metadados, mas esta rodada não executou os projetos em ambientes limpos nem inspecionou integralmente todos os arquivos de todos os 34 repositórios. Por segurança, não foram substituídos módulos de aplicação, dependências ou workflows sem validar seus comandos e contratos. Não foram apagados arquivos, alteradas visibilidades, reescritos históricos ou ativadas configurações financeiras.

## Próxima sequência de trabalho

- Concluir P0 com testes em ambiente limpo, CI compatível, segurança revisada e releases versionadas.
- Depois concluir P1 por stack e domínio.
- Transformar P2 em projetos de pesquisa com critérios mensuráveis.
- Revisar P3 e atribuições de terceiros.
- Atualizar o catálogo institucional somente com evidências já confirmadas.


## Registro de execução verificada

**Atualização:** 22/11/2026.

### Aurora GeoIntelligence XAI
- CI Python 3.11 executado com sucesso no commit `3935b0fd60cec73b6f4b5edab4b5942f0c8699c2`.
- O job confirmou instalação de dependências, validação de sintaxe e execução da suíte de testes.
- Workflows: [GeoIntelligence CI](https://github.com/felipetjmg1-bit/aurora-geointelligence-xai/actions/runs/45037000443) e [CPU CI](https://github.com/felipetjmg1-bit/aurora-geointelligence-xai/actions/runs/45037000376).
- Permanecem pendentes revisão científica, instalação independente, validação com dados reais autorizados, lockfile e release.

### Sentinela Brasil
- Corrigida a dependência opcional de testes de `httpx2` para `httpx` em `pyproject.toml`.
- Workflow atualizado para instalar o extra declarado `.[test]`, evitando dependências de teste duplicadas fora do manifesto.
- CI Python 3.11 executado com sucesso no commit `04abf764061dfea76c518675cfe716bdba0822be`, incluindo instalação do projeto e execução dos testes de API/segurança.
- Evidência: [execução CI](https://github.com/felipetjmg1-bit/sentinela-brasil/actions/runs/45037200324).
- Permanecem pendentes revisão independente de segurança, rotação/backup de chaves, política operacional, hardening de implantação e testes de abuso.

### Oráculo X-37
- Corrigido o padrão de DEBUG para permanecer desativado por padrão em `app/core/config.py` (commit `f037a95e0f58128a0432a3378e8bbe36bbef799f`).
- Substituída a política SECURITY.md genérica por orientações coerentes com o estágio atual de desenvolvimento, incluindo alerta sobre rotas sem autenticação e artefatos pickle.
- Adicionado Dependabot para atualizações semanais de dependências Python e GitHub Actions.
- As execuções CI do commit de documentação e do commit de configuração Dependabot foram disparadas; a conclusão do run mais recente ainda precisa ser conferida.
- Bloqueador técnico: API Flask e servidor MCP não possuem autenticação de produção integrada; não expor publicamente. Manifestos de dependências ainda precisam ser reconciliados e testados em instalação limpa.

**Nota de integridade:** resultados de CI comprovam apenas os comandos executados no workflow e naquele commit. Não constituem certificação, auditoria independente, garantia de segurança ou prontidão para produção.


## Identidade visual e institucional

Em 22/11/2026, os READMEs dos 33 repositórios de projetos foram padronizados para exibir **Impulso Digital Soluções em IA** e incorporar um diagrama SVG próprio de fluxo/funcionalidades em `PROJECT-OVERVIEW.svg`. Os diagramas foram preparados com elementos SVG básicos para compatibilidade com a renderização do GitHub. São mapas explicativos do código/documentação, não screenshots de uma execução real.

Os rótulos públicos de maturidade foram ajustados para descrever entregas e estágios de desenvolvimento, sem declarar conclusão, homologação ou prontidão de produção sem evidência. Repositórios que ainda são documentos de pesquisa ou especificação continuam identificados como tal.
