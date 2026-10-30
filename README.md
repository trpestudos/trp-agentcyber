# 🛡️ TRP Agente Cyber

Este repositório é a entrega do desafio de Cybersecurity da DIO. O objetivo foi evoluir o **DIO Agent** (baseado no Hermes) de um agente genérico para o **TRP Agente Cyber**, um Mentor e Scanner de Segurança especializado em AppSec, capaz de auditar códigos, correlacionar falhas com padrões da indústria e ensinar o usuário a corrigi-las.

## 🎯 A Especialização Escolhida

O projeto base do DIO Agent é capaz de conversar e executar comandos. Nós o especializamos para agir como um **Analista de AppSec**, adicionando a ele uma nova camada de inteligência técnica.

**Por que escolhemos esta especialização?**
No mercado de segurança, não basta encontrar uma falha; é preciso saber *onde* ela se encaixa. O TRP Agente Cyber foi treinado para:
- Identificar a falha técnica.
- Classificá-la segundo o **OWASP Top 10 (versão atual)**.
- Mapear a tática do atacante no **MITRE ATT&CK**.
- Correlacionar com **OSINT** (catálogo CISA KEV e EPSS) para saber se a falha está sendo explorada ativamente no mundo real.

## 🛠️ O que foi criado e alterado

A seguir, os arquivos que compõem a evolução do agente:

### 1. Nova Skill: `scan-vulnerability` (em `skills/scan-vulnerability/`)
Esta é a skill de ação. Ela instrui o agente a realizar varreduras técnicas e gerar relatórios estruturados.
- **`SKILL.md`:** O "cérebro" da skill. Define o processo de 5 etapas (Contexto > Análise > Correlação > Classificação > Remediação) e o formato rígido do relatório.
- **`README.md`:** A documentação humana que explica o que essa skill faz e como testá-la.

### 2. Conhecimento Adicional: `security-basics.md` (em `agent/knowledge/`)
Arquivo com conceitos fundamentais de segurança (Tríade CIA, diferença entre vulnerabilidade, ameaça e risco, e boas práticas).

### 3. Atualização da Persona: `agent/persona.md`
Adicionamos a identidade de "TRP Agente Cyber: Especialista em Segurança e Auditoria", definindo o tom técnico, cético e ético do agente.

### 4. Atualização do `AGENTS.md`
Incluímos a nova skill na tabela de habilidades do agente, para que ele saiba quando acioná-la.

## 🚀 Como Rodar o Agente

1.  Instale o Hermes Agent no seu terminal Linux/macOS:
    ```bash
    curl -fsSL https://hermes-agent.nousresearch.com/install.sh | bash