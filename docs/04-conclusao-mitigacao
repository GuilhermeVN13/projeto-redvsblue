# 🏁 Conclusão e Recomendações de Mitigação

Este laboratório demonstrou a importância das capacidades de monitoramento e detecção de segurança em ambientes modernos. Através da simulação, foi possível compreender como ataques de força bruta se apresentam sob uma perspectiva defensiva e como equipes de SOC podem identificá-los via SIEM.

## 🛡️ Recomendação de Mitigação (Blue Team)

Para remediar as vulnerabilidades exploradas neste lab e as falhas de visibilidade encontradas, propõe-se o seguinte plano de ação:

| Mitigação | Descrição |
| :--- | :--- |
| **Política de Bloqueio de Conta** | Configurar o Windows para bloquear contas automaticamente após X tentativas falhas, prevenindo o Brute-Force. |
| **Restrição RDP** | Limitar o acesso via Firewall apenas para IPs conhecidos ou utilizar uma VPN (Gateway RDP). |
| **Autenticação Multi-fator (MFA)** | Adicionar uma camada extra de segurança além da senha para logins remotos. |
| **Regras de Correlação SIEM** | Implementar regras avançadas no Wazuh para alertar sobre padrões de pós-autenticação suspeitos. |

## 📝 Análise Final de Segurança

O ataque de força bruta gerou múltiplos logs de falha de autenticação que foram detectados com sucesso pelo Wazuh. 

No entanto, uma vez autenticado, os comandos básicos do sistema executados pelo atacante não dispararam alertas. Isso reforça que uma estratégia de defesa eficiente não deve focar apenas no perímetro (o login), mas também no monitoramento contínuo e na análise comportamental de processos dentro da rede.

---
**Autor:** Guilherme Freitas  
**Projeto:** Red vs Blue Team Cybersecurity Lab

---
[⬅️ Voltar para Fase Blue Team](03-fase-defensiva.md) | [🏠 Voltar para o Início](../README.md)
