# Plano de Entrega — Fundação do Produto

**Estado atual:** arquitetura e governança documentadas. A aplicação ainda não foi implementada.

## Objetivo do primeiro produto funcional

Entregar uma fundação utilizável para cadastrar organizações independentes, usuários, permissões, módulos e fluxos de trabalho com agentes. O primeiro piloto será a agência multissetorial. A operação FERRAZ de rochas será integrada como módulo separado somente após auditoria técnica do produto existente.

## Ordem obrigatória

### Fase 0 — decisões e inventário
- Confirmar repositórios, responsáveis, licenças e estado real dos produtos existentes.
- Mapear dependências, dados, autenticação e infraestrutura já disponíveis.
- Definir requisitos de disponibilidade, privacidade, retenção, recuperação e orçamento.
- Escolher stack após comparar o que já existe e o custo de manutenção.

### Fase 1 — núcleo mínimo
- Aplicação web responsiva e autenticação.
- Organização/empresa, usuários, papéis e permissões.
- Isolamento de dados por organização no backend e no banco.
- Cadastro e ativação de módulos.
- Auditoria de ações e histórico.
- Configuração de marca por empresa.
- Ambiente de desenvolvimento, testes e deploy controlado.

### Fase 2 — fluxo de trabalho e qualidade
- Cadastro de clientes, projetos e demandas.
- Tarefas, estados, responsáveis e dependências.
- Registro de versões e arquivos.
- Pipeline executor → editor → revisor → aprovação humana.
- Checklist, reprovação, correção e nova revisão.
- Evidência de testes e trilha de auditoria.

### Fase 3 — agentes
- Catálogo e configuração de agentes.
- Permissões por agente, empresa, módulo e ferramenta.
- Orquestrador com fila, limites, custo e observabilidade.
- Subagentes/DOTs apenas quando houver caso de uso recorrente.
- Proteções contra vazamento de contexto entre empresas.
- Execução paralela somente em tarefas independentes.

### Fase 4 — piloto da agência
- Briefing e diagnóstico do cliente.
- Pesquisa e estratégia.
- Marca e Design System por cliente.
- Projetos de site e conteúdo.
- Campanhas e entregas com editor/revisor.
- Aprovações e relatórios de resultado.

### Fase 5 — módulos especializados
- Auditar o sistema FERRAZ de rochas antes de integrar.
- Definir adaptadores e fronteiras entre o núcleo e o produto setorial.
- Testar migração, permissões, dados e regressão.
- Adicionar novos segmentos conforme demanda real.

## Critérios de aceite antes de produção

1. Testes automatizados de isolamento: usuário da empresa A não lê nem altera dados da empresa B.
2. Testes de papéis e permissões no servidor.
3. Testes do fluxo obrigatório de edição e revisão para todos os agentes.
4. Impossibilidade de autoaprovação e de pular revisão obrigatória.
5. Logs de ações sensíveis e aprovações.
6. Proteção de segredos e credenciais.
7. Backup e procedimento de restauração testado.
8. Testes de acessibilidade e responsividade.
9. Limites de uso e custo por empresa/agente.
10. Documentação que distingue protótipo, teste e produção.

## Decisão técnica ainda pendente

Não fixar framework, banco, provedor de autenticação, hospedagem ou fornecedor de IA apenas por preferência. A escolha será registrada em ADR após inventário do código existente, requisitos de segurança, custos, portabilidade e capacidade de operação.

## Regra de entrega

Uma fase só muda para concluída com código no repositório, revisão independente, testes executados e evidências registradas. Texto de planejamento não equivale a software funcional.
