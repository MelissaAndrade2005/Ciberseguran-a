# Segurança Linux & Ops — Portfólio de Melissa Andrade

Módulo do percurso Activation (Skodji Digital), 8 sessões, realizado em WSL2 (Ubuntu).

| Sessão | Tema | O que fiz |
|---|---|---|
| 01 | Introdução à Arquitetura Linux e Segurança do Sistema de Ficheiros | Explorei a estrutura de diretórios (FHS) e percebi o que cada pasta guarda |
| 02 | Comandos Essenciais de Terminal e CLI | Naveguei no sistema e manipulei ficheiros e pastas pela linha de comandos |
| 03 | Comandos Essenciais de Terminal e CLI (Parte 2) | Usei pipes, redirecionamento, `grep` e `wc` para filtrar e contar texto |
| 04 | Gestão de Utilizadores e Grupos | Criei contas e grupos com `useradd` e `groupadd` |
| 05 | Permissões, Controlo de Acessos e Autenticação | Defini permissões com `chmod` em notação octal, seguindo o menor privilégio |
| 06 | Processos e Monitorização de Sistemas | Identifiquei processos com `ps` e terminei-os com sinais (`kill`) |
| 07 | Proteção de Dados, Backup e Automação | Cifrei e decifrei backups com `openssl` e `tar` |
| 08 | Desafio Final Integrador e Consolidação de Competências | 6/6 missões concluídas (ver `sessao-08`) |

## Desafio final (Sessão 8)

No cenário «Recuperar o Servidor da CVTECH», resolvi as 6 missões:

1. **Explorar:** encontrei a nota oculta com `find`.
2. **Filtrar:** localizei a linha crítica do log com `grep` e contei linhas com `wc -l`.
3. **Permissões:** corrigi o ficheiro de RH para `640`.
4. **Contas:** criei o grupo `auditores` e a conta `auditor`.
5. **Processos:** terminei o indexador com SIGTERM, sem `-9`.
6. **Cofre:** decifrei e extraí o backup cifrado.

Evidências na pasta [`sessao-08`](./sessao-08): relatório final, saída do verificador e captura de ecrã.

## O que aprendi

Neste módulo aprendi a trabalhar no Linux pela linha de comandos e a pensar em segurança em cada passo: quem pode ler, quem pode escrever e o que fica registado. No desafio final juntei tudo num só cenário. Percebi que as opções dos comandos importam (um `kill -9` impede o processo de terminar com calma) e que as passwords nunca devem ficar escritas em relatórios nem no GitHub.
