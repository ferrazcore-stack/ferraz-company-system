# Governança de Agentes — Executor, Editor e Revisor

**Regra obrigatória:** todo agente da plataforma, sem exceção, possui um fluxo de execução, edição e revisão. Nenhum agente entrega trabalho como final sem passar pelas duas verificações.

## 1. Ciclo obrigatório de cada agente

1. **Executor:** interpreta a tarefa, confirma objetivo, contexto, empresa, permissões e critérios de aceite; executa somente o escopo autorizado.
2. **Editor:** recebe a entrega e o briefing original; melhora organização, clareza, consistência, precisão, completude, linguagem, formato e aderência à identidade/ao padrão aplicável. Não pode inventar informação nem mudar o objetivo aprovado.
3. **Revisor independente:** confere o briefing, a entrega original e a versão editada; verifica fatos, cálculos, requisitos, riscos, limites, links, fontes e critérios de aceite. Deve poder reprovar e devolver para correção.
4. **Orquestrador:** acompanha o ciclo, registra os resultados, resolve dependências e encaminha a entrega. Não pode ignorar reprovação nem marcar como aprovado sem evidência.
5. **Aprovação humana:** exigida para decisões estratégicas, gastos, publicações, ações externas, alterações sensíveis, operações irreversíveis ou casos definidos pela política da empresa.

O editor e o revisor não são a mesma função. O revisor não deve simplesmente confirmar o que o editor escreveu. A revisão deve ser independente e baseada em critérios verificáveis.

## 2. Como garantir que isso se aplique a TODOS os agentes

Cada agente deve ter em sua configuração:
- editor responsável ou perfil de edição designado;
- revisor responsável ou perfil de revisão designado;
- critérios de aceite específicos da especialidade;
- ferramentas de edição e verificação permitidas;
- política de devolução para correção;
- regra de escalonamento humano;
- registro de versão e evidências.

O sistema não deve permitir que um agente desative, pule ou aprove a própria revisão. Se não houver editor ou revisor disponível, a tarefa fica como **aguardando revisão**, nunca como concluída.

Para evitar multiplicação desnecessária de agentes, Editor e Revisor podem ser capacidades especializadas compartilhadas e designadas por tarefa, com contexto e critérios específicos de cada agente. A obrigação é individual para cada entrega de cada agente, não a criação automática de centenas de instâncias permanentes.

## 3. Perfis de editor e revisor por especialidade

O perfil designado precisa entender o tipo de entrega:
- Estratégia/comercial: lógica, viabilidade, premissas, riscos, margem, coerência e objetivo.
- Pesquisa/inteligência: qualidade das fontes, atualidade, método, evidência e separação entre fato e hipótese.
- Design/branding: briefing, marca, consistência visual, legibilidade, acessibilidade e Design System.
- Marketing/comunicação: público, mensagem, tom, canal, alegações e adequação cultural.
- Site/UX/UI: requisitos, navegação, responsividade, acessibilidade, conteúdo, SEO público e privacidade.
- Audiovisual: roteiro, direitos de uso, identidade, qualidade técnica, legendas e finalidade.
- Neurociência/experiência: evidência, ética, ausência de manipulação e clareza das recomendações.
- Tecnologia: requisitos, arquitetura, segurança, testes, manutenção e regressões.
- Especialistas setoriais: regras e riscos próprios do segmento e limites profissionais.
- Gestão/processos: viabilidade, responsáveis, prazos, dependências, indicadores e clareza operacional.

## 4. Resultado da revisão

Cada revisão deve produzir um registro estruturado:
- tarefa e empresa;
- agente executor e versão da entrega;
- editor e alterações realizadas;
- revisor e checklist utilizado;
- status: aprovado, aprovado com ressalvas ou reprovado;
- problemas encontrados e severidade;
- correções solicitadas;
- evidências e testes realizados;
- necessidade de aprovação humana;
- responsável e data da aprovação final.

**Aprovado com ressalvas** só pode ser usado quando as ressalvas não comprometem segurança, legalidade, exatidão essencial ou critérios obrigatórios. Caso contrário, reprovar e devolver.

## 5. Independência e conflitos

- Sempre que possível, o revisor deve ser diferente do executor e do editor.
- Em entregas de alto risco, a revisão deve ser feita por pessoa/agente independente, sem conflito de interesse.
- O agente que executou não pode alterar o status de revisão.
- Se executor, editor e revisor discordarem, o orquestrador registra o conflito e pede decisão humana quando necessário.
- Nenhum agente pode remover comentários, evidências ou histórico de revisão para ocultar falhas.

## 6. Trabalho paralelo

O executor pode trabalhar em paralelo com outros agentes quando as tarefas forem independentes. A edição começa quando existe uma entrega identificável. A revisão começa sobre uma versão congelada, identificada por número ou hash. Se houver nova alteração após a revisão, a versão precisa passar novamente pelo fluxo aplicável.

## 7. Checklist mínimo universal

Antes de concluir qualquer tarefa:
- O objetivo original foi atendido?
- A empresa e o contexto corretos foram utilizados?
- As permissões foram respeitadas?
- A informação é verificável e não foi inventada?
- O conteúdo está claro, completo e consistente?
- A identidade e os padrões da empresa foram respeitados?
- Os riscos e limitações foram registrados?
- Os testes ou verificações necessários foram executados?
- O editor registrou a edição?
- O revisor independente registrou o resultado?
- A aprovação humana foi obtida quando exigida?

## 8. Proibição de conclusão fictícia

É proibido declarar que uma tarefa está concluída, testada, publicada, segura ou aprovada sem evidência correspondente. Documentação não é implementação; build não é teste de aceitação; teste local não é prova de produção. O status deve refletir o que realmente ocorreu.
