# Esteira de Implantação

Protótipo web estático em arquivo único para organizar o setor de implantação de software com **login de usuários**, **permissões por perfil**, **troca de senha** e **quadro Kanban por Agente de Implantação**.

## O que existe no protótipo

- **Tela de acesso:** login local para entrada dos Agentes de Implantação e do Supervisor do setor.
- **Perfis de usuário:**
  - **Supervisor:** visualiza todos os clientes da esteira, identifica qual é o Agente de Implantação de cada cliente, filtra por agente, cria usuários para a equipe, redefine senhas e administra permissões.
  - **Agente de Implantação:** visualiza apenas os clientes vinculados ao próprio login e pode trocar a própria senha.
- **CRM operacional:** cadastro de cliente, segmento, contato, prioridade, etapa e próxima ação.
- **Kanban de implantação:** colunas preparadas para refletir a sequência real do processo, começando pelas três etapas definidas até agora.
- **Persistência local:** dados salvos no navegador com `localStorage`.

## Credenciais padrão

### Supervisor
- Usuário: `supervisor`
- Senha: `super123`

### Agentes de Implantação
- Usuário: `ana`
- Senha: `implantacao123`
- Usuário: `joao`
- Senha: `implantacao123`

## Fluxo da esteira atual

1. Diagnóstico
2. Estruturação
3. Treinamento - Módulo Comercial

> A sequência dos próximos módulos poderá ser adicionada depois, conforme você passar o restante do fluxo.

## Como usar

1. Abra o arquivo `index.html` em um navegador.
2. Entre com um dos usuários padrão.
3. Cadastre clientes no formulário lateral vinculando cada conta a um Agente de Implantação.
4. Movimente os cards entre as colunas conforme a implantação evolui.
5. Use o painel **Segurança e senha** para trocar sua senha.
6. Se entrar como Supervisor, use a área de usuários para criar acessos, redefinir senhas e acompanhar qual Agente de Implantação está em cada cliente.

## Próxima melhoria sugerida

Depois de fechar toda a sequência dos módulos, a melhoria mais útil será incluir **SLA por etapa**, **motivo de bloqueio** e **data da próxima ação** para cada cliente.

## Observação importante

Este projeto continua sendo um **protótipo front-end**. A autenticação é apenas local e não substitui um backend real com banco de dados, criptografia de senha e controle de sessão seguro.
