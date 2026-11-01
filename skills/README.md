# Skills do TRP Agente Cyber

## O que é uma skill

Uma **skill** é um guia passo a passo que ensina o agente a executar uma tarefa específica bem feita. Em vez de deixar o agente improvisar, a skill dá um processo claro e seguro.

Cada skill fica em uma pasta com um arquivo `SKILL.md`. Esse formato segue o padrão aberto de skills para agentes, então funciona em diferentes harnesses.

## Como o agente usa as skills

O usuário não precisa "chamar" a skill. Basta conversar de forma natural. O agente identifica a necessidade e aplica a skill certa por trás dos panos.

Por exemplo, se o usuário diz "encontrei uma falha estranha nesse código", o agente usa a skill de análise de vulnerabilidades.

## Skills disponíveis

| Skill | Para que serve | Exemplo de pedido do usuário |
|-------|----------------|--------------------------------|
| `study-plan` | Montar um plano de estudos organizado | "Quero ser dev back-end, por onde começo?" |
| `unblock-challenge` | Destravar um desafio sem entregar a resposta | "Travei nesse desafio, me ajuda?" |
| `explain-concept` | Explicar um conceito de forma didática | "Não entendi o que é uma API." |
| `web-search` | Fundamentar respostas com busca atual e fontes citadas | "Qual a versão estável do Node hoje?" |
| `vulnerability-analysis` | Ensinar conceitos de segurança e avaliar riscos | "Como funciona um ataque de SQL Injection?" |
| `scan-vulnerability` | Varredura técnica de código/infra com relatório de risco | "Escaneie esse arquivo e me dê um laudo de segurança." |
| `secure-remediation` | Aplicar correção de vulnerabilidade e validar com testes | "Corrija essa falha e me mostre os testes." |
| `network-recon` | Reconhecimento de rede com correlação MITRE ATT&CK | "Faça um scan de portas no IP X." |
| `portfolio-review` | Revisar portfólio de segurança e currículo técnico | "Revise meu portfólio de AppSec." |

## Como criar uma nova skill

1. Crie uma pasta dentro de `skills/` com um nome curto em inglês.
2. Adicione um arquivo `SKILL.md` com o cabeçalho e o processo (siga o modelo das skills existentes).
3. Adicione a skill na tabela de `AGENTS.md` para o agente saber quando usá-la.
