# Empresas, Módulos e Isolamento de Dados

## 1. Estrutura configurável

A plataforma deve separar quatro conceitos:
- **Plataforma:** infraestrutura e serviços comuns.
- **Organização/empresa:** entidade que contrata e administra seu espaço.
- **Marca/produto:** identidade e oferta que pertencem à empresa.
- **Módulo:** conjunto de funcionalidades ativado para uma empresa ou segmento.

Uma empresa pode ter várias marcas e módulos. Um módulo pode ser disponibilizado a várias empresas, mas cada empresa mantém sua própria configuração e seus próprios registros.

## 2. Isolamento obrigatório

Cada registro privado deve estar associado a uma organização/empresa. A validação de acesso deve ocorrer no backend e no banco de dados, não apenas na interface.

Separar:
- usuários e equipes;
- clientes e contatos;
- projetos e tarefas;
- arquivos e documentos;
- prompts, memória e contexto dos agentes;
- configurações de marca e Design System;
- integrações e credenciais;
- relatórios, métricas e histórico;
- propostas, campanhas e dados comerciais.

Nenhum agente, funcionário ou cliente pode consultar dados de outra empresa sem autorização específica e auditável.

## 3. Serviços compartilhados

Podem ser compartilhados como capacidade da plataforma:
- autenticação e gestão de permissões;
- biblioteca de componentes e tokens de Design System;
- editor e revisor;
- orquestração e catálogo de agentes;
- mecanismos de pesquisa e análise;
- notificações;
- armazenamento via adaptadores;
- observabilidade e controle de custos.

Compartilhar a capacidade não significa compartilhar conteúdo privado. Por exemplo, o motor de Design System pode ser comum, mas logotipos, tokens de marca, arquivos e projetos são isolados por empresa.

## 4. Módulos setoriais

### Agência de Design e Marketing
Pode atender clientes de vários segmentos. Deve permitir cadastrar cliente, briefing, diagnóstico, pesquisa, estratégia, marca, sites, campanhas, conteúdos, entregas, aprovações, orçamento, cronograma e resultados.

Cada cliente deve ter workspace, marca, permissões, arquivos e histórico separados. A agência pode compartilhar métodos e modelos, mas não deve reutilizar dados confidenciais de um cliente em outro.

### FERRAZ — Rochas Naturais e Marmoraria
É um produto/módulo especializado dentro da plataforma mais ampla. Deve preservar sua identidade e seu domínio: clientes, obras, ambientes, materiais, peças, medições, paginação, orçamentos, fornecedores, produção, instalação, documentos e histórico.

O sistema existente de rochas deve ser auditado antes de qualquer integração. Não apagar, reescrever nem substituir cálculos, motor de paginação, regras ou dados existentes sem plano, testes e autorização.

### Novos segmentos
A inclusão de um segmento exige:
- necessidade e público definidos;
- regras e entidades próprias;
- especialista setorial e critérios de revisão;
- permissões e dados isolados;
- fluxo e critérios de aceite;
- avaliação de custos, riscos e manutenção.

## 5. Acesso e administração

Papéis sugeridos, configuráveis:
- administrador da plataforma;
- administrador da empresa;
- gestor de módulo;
- membro da equipe;
- colaborador externo;
- cliente/portal de leitura;
- agente de serviço com escopo técnico limitado.

Acesso de suporte ou administração da plataforma não implica acesso automático a dados privados de clientes. Acesso excepcional deve ser temporário, justificado, autorizado e registrado.

## 6. Configuração por empresa

Cada empresa pode configurar:
- nome, logotipo, cores, tipografia e identidade;
- módulos ativos;
- usuários e funções;
- fluxos, campos e status;
- agentes disponíveis e ferramentas autorizadas;
- editor e revisor responsáveis por cada especialidade;
- limites de autonomia e aprovações;
- integrações, notificações e orçamento;
- políticas de dados, retenção e compartilhamento.

## 7. Critérios mínimos de aceite

- Empresa A não consegue acessar registros, arquivos, memória ou integrações da Empresa B.
- Alterar a empresa ativa não permite reutilizar permissões de outra sessão.
- APIs e consultas verificam tenant e papel no servidor.
- Agentes recebem somente o contexto necessário à tarefa e à empresa correta.
- URLs de arquivos privados não são públicas permanentes.
- A troca de tema/marca de uma empresa não afeta outras.
- Editor e revisor não recebem acesso além do necessário para revisar a entrega.
- A remoção de um usuário revoga suas sessões e acessos conforme política.
- Acesso administrativo excepcional fica registrado.
