# Plataforma Multissetorial — Carta e Arquitetura Mestre

**Status:** proposta inicial para revisão da fundadora.  
**Escopo desta etapa:** arquitetura e definição de responsabilidades; ainda não é implementação de software.

## 1. O que é a plataforma

Uma plataforma empresarial multissetorial, independente de uma marca específica, configurável e expansível. Ela oferece uma base comum para empresas, equipes, projetos, serviços, módulos especializados, agentes e integrações.

A plataforma não é “a plataforma da FERRAZ”. A FERRAZ será uma das empresas/operações que poderá utilizá-la, com seus próprios dados, identidade, usuários, permissões, processos e módulos.

## 2. Camadas da solução

1. **Núcleo da plataforma:** identidade, empresas, usuários, permissões, configurações, auditoria, integrações, notificações e governança.
2. **Orquestração de agentes:** recebe demandas, identifica contexto e permissões, distribui tarefas, acompanha execução e consolida entregas.
3. **Serviços compartilhados:** design system, arquivos, pesquisa, comunicação, gestão de projetos, editor, revisor, métricas e automações.
4. **Módulos de negócio:** funcionalidades específicas ativadas conforme a empresa e o setor.
5. **Aplicações e portais:** interfaces internas, áreas de clientes e sites públicos, cada qual com permissões e identidade adequadas.

## 3. Empresas e produtos dentro da plataforma

A plataforma deve permitir cadastrar diferentes empresas e organizações. Cada uma pode ativar módulos próprios ou compartilhados, sem ser obrigada a usar tudo.

Exemplos iniciais:
- **Agência de Design e Marketing multissetorial:** atendimento a clientes de diversos ramos; estratégia, pesquisa, branding, design, sites, marketing, conteúdo, audiovisual, comunicação e eficiência.
- **FERRAZ — rochas naturais e marmoraria:** operação especializada que deverá ser integrada ou conectada ao produto existente, preservando seus cálculos, fluxos, dados e histórico.
- **Novos módulos setoriais:** poderão ser adicionados para outros segmentos quando houver necessidade validada.

A lista é expansível. Nenhum segmento de exemplo deve ser considerado compromisso de desenvolvimento sem priorização.

## 4. Núcleo compartilhado

O núcleo deverá oferecer, por etapas:
- Cadastro de organizações, empresas, unidades e marcas.
- Usuários, equipes, convites, funções e permissões.
- Separação lógica e técnica dos dados por empresa.
- Cadastro de clientes, contatos, projetos, demandas e entregas.
- Gestão de documentos, versões, aprovações e histórico.
- Configuração de módulos, fluxos, campos e status.
- Design System e temas independentes por marca.
- Central de agentes, tarefas, ferramentas e supervisão.
- Editor e revisor integrados aos fluxos de trabalho.
- Auditoria, notificações, métricas e controle de custos.
- Integrações externas com credenciais protegidas.

## 5. Agência de Design e Marketing

A agência é um módulo/negócio multissetorial dentro da plataforma, não o limite da plataforma inteira.

Competências a cobrir:
- Estratégia e planejamento comercial.
- Inteligência e pesquisa de mercado.
- Branding, posicionamento e arquitetura de marca.
- Direção de arte e Design System.
- Design gráfico, apresentações e materiais comerciais.
- Planejamento de marketing, campanhas e canais.
- Comunicação, conteúdo e relacionamento.
- Criação e desenvolvimento de sites e páginas.
- UX/UI, acessibilidade e experiência digital.
- Produção, edição e tratamento de imagens e vídeos.
- Eficiência de processos e análise de resultados.
- Neurociência e psicologia aplicadas à comunicação, comportamento e experiência, com base em evidências e sem manipulação.

O fluxo deve cobrir a jornada completa: receber a necessidade → entender o negócio → pesquisar → diagnosticar → propor estratégia → apresentar para aprovação → planejar → criar → revisar → executar o que foi autorizado → acompanhar → medir → registrar aprendizados.

A agência não deve ser reduzida a uma fábrica de posts, nem assumir automaticamente serviços jurídicos, contábeis, médicos ou outras atividades regulamentadas. Não promete resultados garantidos e não publica, contrata, compra ou assume compromissos em nome do cliente sem autorização específica.

## 6. Neurociência aplicada

É uma competência transversal, não uma justificativa para criar um agente para cada tarefa. Pode apoiar:
- clareza e compreensão da informação;
- arquitetura de informação e experiência do usuário;
- atenção, percepção e carga cognitiva;
- comportamento do consumidor e tomada de decisão;
- comunicação ética e acessível;
- testes de experiência e interpretação cuidadosa de resultados.

Toda afirmação deve distinguir evidência, hipótese e recomendação. Não usar manipulação, exploração de vulnerabilidades, falsas urgências ou alegações científicas sem fonte adequada.

## 7. Estrutura inicial de competências e agentes

A estrutura inicial deve ser enxuta e evoluir conforme demanda comprovada:
- Orquestrador central e governança.
- Produto, requisitos e processos.
- Estratégia empresarial e comercial.
- Inteligência, pesquisa e dados.
- Design, marca e experiência.
- Marketing, comunicação e audiovisual.
- Tecnologia, arquitetura e integrações.
- Especialistas setoriais, ativados por módulo.
- Segurança, privacidade e conformidade.
- Qualidade: edição, revisão e testes.

Esses nomes representam responsabilidades. Não obrigam a criar um agente separado para cada item. Competências relacionadas podem ser agrupadas. Subagentes e DOTs só serão criados quando houver escopo, ferramentas, carga de trabalho e critérios de qualidade claros.

## 8. DOTs, agentes e subagentes

- **Orquestrador:** recebe a demanda, identifica a empresa e o módulo, verifica permissões, divide o trabalho e coordena dependências.
- **Agente especialista:** responde por uma competência e produz entregas dentro de seu escopo.
- **Subagente:** executa uma parte delimitada do trabalho de um especialista.
- **DOT:** unidade especializada configurável, com missão, limites, ferramentas e métricas próprias.
- **Editor:** melhora a entrega do agente, conferindo estrutura, clareza, consistência, completude e aderência ao briefing.
- **Revisor:** faz uma verificação independente, testa critérios de aceite, identifica erros e registra aprovação ou reprovação.

Todo agente, sem exceção, deverá passar por editor e revisor antes de sua entrega ser considerada final. Detalhes no documento de governança.

## 9. Trabalho simultâneo

A plataforma poderá executar tarefas em paralelo quando forem independentes. O orquestrador deve:
- identificar dependências;
- dividir entregas com limites claros;
- impedir que dois agentes alterem o mesmo artefato sem coordenação;
- consolidar resultados;
- encaminhar conflitos e decisões relevantes à pessoa responsável.

Tarefas dependentes devem respeitar a sequência. Paralelismo não significa ausência de coordenação.

## 10. Governança e autonomia

A autonomia deve ser configurada por empresa, módulo, agente, ferramenta e tipo de ação.

Modos:
1. Consultar e observar.
2. Analisar e recomendar.
3. Preparar rascunhos.
4. Executar tarefas internas reversíveis previamente autorizadas.
5. Solicitar aprovação antes de publicar, enviar, contratar, comprar, alterar dados sensíveis ou assumir compromissos externos.

A aprovação humana deve ser explícita para ações estratégicas, financeiras, externas, irreversíveis ou de alto impacto. Toda ação relevante registra solicitante, agente, editor, revisor, empresa, versão, aprovação, data, resultado e falhas.

## 11. Isolamento e segurança

- Cada registro operacional pertence a uma empresa/tenant.
- Cada consulta, gravação, arquivo, agente e ferramenta deve validar empresa e permissão no servidor.
- Agentes não podem usar dados de uma empresa em benefício ou resposta de outra.
- Memória, arquivos, prompts privados, métricas e histórico devem respeitar a separação por empresa e finalidade.
- Catálogos compartilhados devem ser explicitamente definidos como compartilhados e, por padrão, somente leitura.
- Segredos nunca ficam no código, nos prompts públicos ou no navegador.
- Negar acesso por padrão e registrar acessos excepcionais.
- A plataforma não deve alegar conformidade legal ou segurança certificada sem avaliação e evidências.

## 12. Design System e sites

A plataforma terá um sistema visual central de componentes e tokens, com possibilidade de temas e identidades independentes por empresa/produto.

Cada site ou aplicação deve ter:
- objetivo, público e jornada definidos;
- marca e conteúdo aprovados;
- responsividade, acessibilidade e desempenho;
- SEO apenas para conteúdo público;
- isolamento de painel, dados e arquivos privados;
- editor e revisor para conteúdo, interface e acessibilidade;
- aprovação antes de publicação.

Não impor a identidade FERRAZ a outras empresas. O Design System compartilhado define padrões técnicos; cada marca controla sua própria expressão visual.

## 13. O que fica fora do escopo automático

A plataforma não deve:
- ser exclusiva da FERRAZ;
- misturar dados ou identidades de clientes;
- obrigar todos os setores a usar o mesmo fluxo;
- criar dezenas de agentes sem necessidade;
- permitir que agentes se autoaprovem;
- publicar ou executar ações externas sem autorização adequada;
- inventar dados, pesquisas, custos, resultados ou fontes;
- substituir profissionais habilitados;
- reconstruir módulos especializados que já funcionem sem auditoria;
- assumir que a existência de documentação significa que o recurso está implementado;
- escolher fornecedor, tecnologia ou plano pago sem avaliação de requisitos, custos, limites e aprovação.

## 14. Sequência de construção

1. Validar esta arquitetura e o vocabulário da plataforma.
2. Inventariar os repositórios e sistemas existentes.
3. Mapear o que será núcleo compartilhado, produto independente ou módulo setorial.
4. Definir modelo multiempresa, identidade, permissões e auditoria.
5. Definir o catálogo de agentes com editor e revisor obrigatórios.
6. Construir a fundação técnica mínima e testá-la.
7. Implementar primeiro um fluxo piloto da agência multissetorial.
8. Integrar a FERRAZ de rochas como módulo/produto independente, sem perder o que já existe.
9. Adicionar novos setores por prioridade e validação.
10. Testar segurança, qualidade, custos, usabilidade e recuperação antes de produção.

## 15. Critério de verdade

Documentação, protótipo, código, teste e produção são estados diferentes. Toda entrega deve informar claramente em qual estado está. Nenhum recurso pode ser apresentado como funcional sem evidência de implementação e teste.
