<div align="center">
  <img src="https://github.com/Gus4Dev/Demoday---Skane/blob/main/WhatsApp%20Image%202026-11-12%20at%2022.39.08.jpg?raw=true" alt="Logo SKANE" width="220" />
  <h1>SKANE</h1>
  <p><strong>"A bomba não diz, mas o seu carro sente."</strong></p>
</div>

---

## 📌 Apresentação do Projeto
A **SKANE** é uma solução automotiva inteligente desenvolvida para devolver a transparência e a segurança financeira aos motoristas no momento do abastecimento. Por meio de hardware embarcado e um aplicativo intuitivo, o sistema monitora os dados reais do veículo em tempo real.

## ❗ Problema Identificado
Motoristas enfrentam diariamente a desconfiança em relação à quantidade de combustível efetivamente adicionada ao tanque nos postos de abastecimento. Além do prejuízo financeiro direto, há grande dificuldade em acompanhar métricas reais de consumo e saúde básica do veículo de forma simples.

## 💡 Solução Proposta
Um dispositivo automotivo compacto conectado diretamente à porta **OBD-II** do veículo (utilizando um adaptador **ELM327**), que transmite os dados de telemetria via **Bluetooth** para o aplicativo mobile da SKANE, realizando cálculos comparativos antes e depois do abastecimento.

## ⚙️ Funcionalidades
* **Auditoria Estimada do Tanque:** Leitura precisa do sensor de nível de combustível via OBD-II.
* **Comparação Pré e Pós-Abastecimento:** Registro automático do volume antes de abastecer e verificação imediata após o término.
* **Estimativa de Litros Adicionados:** Cálculo comparativo entre o que foi pago na bomba e o que realmente entrou no tanque.
* **Informações do Veículo:** Painel com dados de telemetria e diagnósticos básicos.
* **Comunidade de Alertas:** Sistema colaborativo de avaliações e alertas sobre postos de combustível.

> ⚠️ **Limitação Técnica:** A SKANE estima os litros adicionados exclusivamente a partir dos sensores eletrônicos disponíveis na central do veículo (ECU/OBD-II). O sistema **não comprova** adulteração ou composição química do combustível.

## 💼 Modelo de Negócio
* **Hardware:** Venda direta do dispositivo OBD-II SKANE.
* **Freemium:** Funcionalidade básica de auditoria de abastecimento gratuita no aplicativo.
* **Assinatura Premium:** Histórico avançado, relatórios detalhados de consumo e alertas prioritários da comunidade.

---

## 🏗️ Arquitetura do Sistema
O ecossistema SKANE opera em uma arquitetura modular desacoplada:
1. **Hardware (OBD-II / ELM327):** Coleta os PIDs (dados) da ECU do veículo.
2. **Mobile (Front-end):** Recebe os pacotes via Bluetooth, exibe ao motorista e envia os registros para a API.
3. **API (Back-end):** Processa os cálculos de diferença de litragem, armazena o histórico e gerencia a comunidade.
4. **Módulo de Acesso:** Gerencia fluxos isolados de autenticação e recuperação de senha por e-mail.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Linguagens:** Python, JavaScript, HTML5, CSS3, SQL
* **Frameworks e Bibliotecas:** FastAPI, React Native
* **Banco de Dados:** MySQL
* **Hardware & Protocolos:** OBD-II, ELM327, Bluetooth
* **Versionamento:** Git, GitHub

---

## 📊 Distribuição de Linguagens (GitHub Linguist)
*(Nota: Atualize os valores abaixo com os números exatos exibidos na barra lateral direita "Languages" do seu repositório no GitHub após o upload).*

| Linguagem | Participação |
| :--- | :--- |
| **Python** | `XX%` |
| **JavaScript** | `XX%` |
| **HTML** | `XX%` |
| **CSS** | `XX%` |

---

## 📂 Estrutura do Ecossistema (Repositórios Relacionados)
O projeto está dividido em quatro repositórios principais para facilitar a manutenção e escalabilidade:

* 📘 **[SKANE — Demoday](https://github.com/Gus4Dev/Demoday---Skane):** Documentação geral, visão de negócio e arquitetura (Você está aqui).
* 📱 **[SKANE — Front-end](#):** Aplicativo mobile desenvolvido em React Native.
* ⚙️ **[SKANE — Back-end](#):** API RESTful em Python/FastAPI, regras de negócio e cálculos.
* 🔐 **[SKANE — Recuperação de E-mail](#):** Módulo responsável pela recuperação de credenciais e segurança de acesso.

---

## 👥 Equipe e Funções
* **[Nome do Integrante 1]** — [Função, ex: Back-end & Arquitetura]
* **[Nome do Integrante 2]** — [Função, ex: Front-end & UI/UX]
* **[Nome do Integrante 3]** — [Função, ex: Hardware OBD-II & Dados]
* **[Nome do Integrante 4]** — [Função, ex: Negócios & Documentação]

## 🙏 Agradecimentos
Agradecemos aos professores, mentores e organizadores do Demoday pelo suporte técnico, orientações de negócio e incentivo durante todo o desenvolvimento da SKANE.
