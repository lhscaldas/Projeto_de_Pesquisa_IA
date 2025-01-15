# Estrutura do Projeto de Pesquisa

- **Título:** Implementação de um método baseado em aprendizado por reforço para otimizar a comunicação peer-to-peer entre uma embarcação autônoma da Marinha do Brasil (VSNT-LAB) e um navio-mãe.}
- **Orientadora:** Profa. Rosa Maria Meri Leão

## 1. Introdução
- **Contextualização**:
  - Apresente o USV-Lab como uma plataforma da Marinha do Brasil para pesquisa e desenvolvimento em veículos autônomos marítimos.
  - Destaque a importância da comunicação eficiente e resiliente em missões autônomas, como as realizadas durante o exercício MINEX-23.
  - Explique os desafios de manter comunicações peer-to-peer confiáveis entre o navio-mãe e o USV-Lab em cenários de operações críticas.

- **Problema**:
  - Identifique problemas como latência, perda de pacotes e falhas de comunicação em canais mesh e VPN, que comprometem a autonomia e a eficiência das missões.

- **Justificativa**:
  - Ressalte como a pesquisa contribui para a robustez das operações autônomas e para a segurança em missões militares e civis, alinhada aos interesses estratégicos da Marinha no "Amazônia Azul".

---

## 2. Revisão da Bibliografia
- **Sistemas de Navegação Marítima Autônoma**:
  - Discuta o uso de frameworks como MOOS-IvP para controle e decisão autônoma.
  - Inclua comparações entre abordagens de controle autônomo e controle humano.

- **Comunicação Peer-to-Peer em Veículos Marítimos**:
  - Explore desafios de comunicação em redes mesh e VPNs, incluindo limitações de largura de banda e latência.

- **Modelagem de QoS com HMM e RL**:
  - Revise estudos que aplicam Cadeias de Markov Ocultas (HMM) e Aprendizado por Reforço (RL) para prever e otimizar a qualidade de serviço em redes heterogêneas.

- **Aplicações Militares de Redes Autônomas**:
  - Aborde o uso de Edge Computing para processamento a bordo e minimização de dependência de tráfego de dados.

---

## 3. Objetivos
- **Objetivo Geral**:
  - "Desenvolver e implementar um método baseado em aprendizado por reforço para otimizar a comunicação peer-to-peer entre o navio-mãe e o USV-Lab, utilizando múltiplos canais de comunicação (mesh e VPN)."

- **Objetivos Específicos**:
  - Caracterizar os desafios de comunicação específicos do USV-Lab.
  - Coletar dados de desempenho dos canais mesh e VPN durante missões simuladas e reais.
  - Modelar as condições de rede com HMM, considerando diferentes cenários operacionais.
  - Implementar um algoritmo de RL para gerenciar e otimizar a troca entre canais.
  - Validar o método em operações no ambiente marítimo, incluindo exercícios supervisionados pela Marinha.

---

## 4. Metodologia
1. **Descrição do Sistema**:
   - Apresente os componentes do USV-Lab relevantes para a comunicação, como sensores, atuadores e infraestrutura de rede (baseada em mesh e VPN via 4G).
   - Explique a integração com o framework MOOS-IvP.

2. **Coleta de Dados**:
   - Descreva os experimentos para coletar métricas de QoS (latência, perda de pacotes, jitter) durante missões simuladas e reais.

3. **Modelagem com HMM**:
   - Utilize HMM para identificar estados ocultos de rede, como "rede boa", "rede degradada" e "rede indisponível".

4. **Implementação de RL**:
   - Defina o MDP (estados, ações, recompensas) para gerenciar dinamicamente a troca entre os canais mesh e VPN.

5. **Validação**:
   - Teste o método em cenários reais, como operações militares e simulações na Baía de Guanabara e na Baía de Todos os Santos.

6. **Ferramentas e Tecnologias**:
   - Detalhe as tecnologias usadas, incluindo MOOS-IvP, infraestrutura de rádio mesh e VPN, e algoritmos de RL.

---

## 5. Conclusão
- **Resultados Esperados**:
  - Otimização do uso dos canais de comunicação, garantindo maior resiliência e eficiência nas missões do USV-Lab.
  - Validação da aplicabilidade de HMM e RL em cenários marítimos críticos.

- **Impacto do Projeto**:
  - Contribuir para a evolução das capacidades autônomas da Marinha do Brasil.
  - Aumentar a confiabilidade e eficiência em operações de defesa e pesquisa marítima.

- **Trabalhos Futuros**:
  - Expandir o método para incluir mais canais de comunicação, como links satelitais.
  - Integrar algoritmos de fusão de sensores para melhorar a qualidade dos dados de QoS.
