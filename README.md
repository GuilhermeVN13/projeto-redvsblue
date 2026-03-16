# 🛡️ Laboratório de Cibersegurança: Red vs Blue

**Autor:** Guilherme Freitas  
**Foco:** Reprodução e detecção de ataque de força bruta no protocolo RDP

## 📝 Resumo do Projeto
Este projeto demonstra a construção de um lab de cibersegurança caseiro para simular tarefas de Blue Team (defesa) e Red Team (ataque).

O cenário foca em um erro humano: uma máquina Windows 11 configurada incorretamente, que sofre um ataque de força bruta disparado de um ParrotOS, sendo tudo monitorado por um SIEM Wazuh.

## 🏗️ Arquitetura do Ambiente
O laboratório foi construído utilizando VirtualBox com a seguinte estrutura de rede:

* **Host (Blue Team):** Kali Linux rodando o Wazuh Manager via Docker.
* **Atacante (Red Team):** ParrotOS (IP: 10.10.10.10).
* **Vítima (Target):** Windows 11 (IP: 10.10.10.20) com Wazuh Agent e RDP habilitado.

## 🛠️ Ferramentas Utilizadas
* **SIEM:** Wazuh
* **Scanner:** Nmap
* **Ataque:** Hydra
* **Acesso Remoto:** FreeRDP
* **Virtualização:** VirtualBox

## 🔗 Navegação do Projeto
Acompanhe o detalhamento técnico de cada etapa:

1. [🌐 Configuração da Rede e Adaptadores](docs/01-configuracao-rede.md)
2. [🔥 Fase Red Team: Ataque e Exploração](docs/02-fase-ofensiva.md)
3. [🛡️ Fase Blue Team: Detecção e Alertas](docs/03-fase-defensiva.md)
4. [🏁 Análise de Segurança e Mitigações](docs/04-mitigacao-conclusao.md)

---
**Objetivo:** Demonstrar habilidades práticas com ferramentas open-source e criar uma base para práticas futuras focadas em Purple Team.


## 🚀 Próximos Passos (Roadmap de Testes)

Este repositório continuará sendo atualizado com novos laboratórios e testes de cibersegurança. Os próximos temas previstos são:

- [ ] **Persistência em Windows:** Criação de serviços e chaves de registro para manter acesso pós-exploração.
- [ ] **Escalação de Privilégio:** Exploração de vulnerabilidades de kernel e configurações incorretas (Misconfigurations) para obter privilégios de `SYSTEM`.
- [ ] **Detecção Avançada (Sysmon):** Integração do Sysmon com o Wazuh para monitoramento detalhado de criação de processos e conexões de rede.
- [ ] **Análise de Malware:** Simulação de execução de Ransomware em ambiente controlado para observar os alertas no SIEM.
- [ ] **Hardening Automatizado:** Uso de scripts PowerShell e GPO para aplicar as mitigações sugeridas de forma automática.

---
