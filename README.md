<div align="center">

<img alt="Kaio Felix de Oliveira — Tech Lead &amp; Software Architect" src="https://capsule-render.vercel.app/api?type=waving&color=0:0A66C2,100:6E4AFF&height=170&section=header&text=Kaio%20Felix%20de%20Oliveira&fontSize=40&fontColor=ffffff&fontAlignY=34&desc=Tech%20Lead%20%26%20Software%20Architect&descAlignY=54&descSize=16&animation=fadeIn" />

<a href="https://www.linkedin.com/in/kaio-felix-oliveira/">
  <img alt="Tech Lead &amp; Software Architect · Java, Spring Boot, Kafka e AWS · arquitetura event-driven em produção" src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=0A66C2&center=true&vCenter=true&width=720&height=45&lines=Tech+Lead+%26+Software+Architect;Java+%7C+Spring+Boot+%7C+Kafka+%7C+AWS;Arquitetura+event-driven+em+produ%C3%A7%C3%A3o;Do+backend+ao+app+que+o+usu%C3%A1rio+usa" />
</a>

<p>
  <a href="https://www.linkedin.com/in/kaio-felix-oliveira/">
    <img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:kaio.felix.oliveira.mail@gmail.com">
    <img alt="E-mail" src="https://img.shields.io/badge/E--mail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://kaiofelixdeoliveira.github.io/">
    <img alt="Portfólio" src="https://img.shields.io/badge/Portf%C3%B3lio-111827?style=for-the-badge&logo=githubpages&logoColor=white" />
  </a>
  <img alt="Visitas no perfil" src="https://komarev.com/ghpvc/?username=kaiofelixdeoliveira&style=for-the-badge&color=0A66C2&label=Perfil" />
</p>

</div>

---

## 🧭 Escolha por onde começar

> Clique na seção que combina com você — cada uma leva menos de um minuto.

<details>
<summary><b>🧑‍💼 Sou gestor ou recrutador</b> — o resumo em 30 segundos</summary>

<br/>

**O que eu entrego**

| | |
| --- | --- |
| 🏗️ **Arquitetura que sustenta o negócio** | Desenho serviços em Java/Spring Boot com Clean Architecture, separando domínio de infraestrutura — para que trocar banco, fila ou provedor não vire um projeto de seis meses. |
| 🔄 **Integrações que não derrubam o sistema** | Comunicação assíncrona com Kafka e RabbitMQ: quando um serviço cai, a fila segura o baque em vez de o cliente ver erro. |
| 🚀 **Entrega previsível** | Pipelines de CI/CD no Azure DevOps tiram o deploy do caminho crítico do time — menos "sexta-feira de subida", mais rotina. |
| 🧩 **Produto de ponta a ponta** | Quando o time precisa, vou do backend ao front (React, Angular) e ao mobile (Flutter). Entrego o que o usuário usa, não só o endpoint. |
| 🤝 **Time mais forte do que quando cheguei** | Trade-offs documentados, code review como parte da entrega e mentoria de devs em início de carreira. |

**Como eu trabalho com stakeholders**

- Traduzo decisão técnica em consequência de negócio: prazo, custo e risco — não em jargão.
- Prefiro dizer "esse caminho nos custa X em manutenção" antes de escrever a primeira linha.
- Entrego em fatias que dá para validar, em vez de um big bang no fim do trimestre.

📄 Currículo completo e histórico profissional no **[LinkedIn](https://www.linkedin.com/in/kaio-felix-oliveira/)**.

</details>

<details>
<summary><b>👨‍💻 Sou dev ou tech lead</b> — como eu construo software</summary>

<br/>

**Uma arquitetura de referência que costumo aplicar:**

```mermaid
flowchart LR
    U["🌐 Web / 📱 Mobile"] -->|REST| GW["API Gateway"]
    GW --> SVC["Serviço de Domínio<br/>Spring Boot"]
    SVC -->|publica evento| K[("Apache Kafka")]
    K --> PROC["Processamento<br/>assíncrono"]
    K --> NOTIF["Notificações"]
    SVC --> DB[("PostgreSQL")]
    PROC --> DB
    LEG["Sistema legado"] <-->|SOAP| SVC
    SVC -.->|métricas e logs| OBS["Observabilidade"]

    classDef core fill:#0A66C2,stroke:#0A66C2,color:#fff
    classDef edge fill:#6E4AFF,stroke:#6E4AFF,color:#fff
    class SVC,PROC,NOTIF core
    class GW,K edge
```

**Princípios que eu levo a sério**

- **O domínio não conhece o framework.** Se trocar Spring por outra coisa quebra a regra de negócio, o desenho está errado.
- **Evento é contrato.** Mudança de payload é versionada, não é "ajuste rápido em produção".
- **Idempotência não é opcional** em consumidor de fila — reprocessamento acontece.
- **Legado se isola, não se xinga.** Camada anticorrupção sobre o SOAP e o resto do sistema segue evoluindo.
- **Teste é documentação executável.** Se o caso de uso não tem teste, ele não está pronto.

**Onde ver isso no código:** [`clean-architeture-album`](https://github.com/kaiofelixdeoliveira/clean-architeture-album) (camadas e casos de uso) · [`kafka-consumer`](https://github.com/kaiofelixdeoliveira/kafka-consumer) (consumo de eventos) · [`starter-webservice-soap`](https://github.com/kaiofelixdeoliveira/starter-webservice-soap) (integração com legado).

</details>

<details>
<summary><b>🔭 No que estou trabalhando agora</b></summary>

<br/>

Um **ecossistema de saúde e nutrição** — API, aplicativo mobile e painel web para profissionais — com apoio de IA no acompanhamento do paciente.

É o tipo de problema que gosto: domínio com regras de verdade, múltiplos clientes consumindo o mesmo núcleo e dados que precisam estar certos, não só disponíveis.

</details>

<details>
<summary><b>☕ Fora do código</b></summary>

<br/>

- 📚 Leitura recorrente: arquitetura de software, sistemas distribuídos e tudo que ajude a errar menos em decisão cara de reverter.
- 🧪 Gosto de montar provas de conceito pequenas antes de defender uma escolha técnica — daí vêm boa parte dos repositórios aqui.
- 💬 Sempre aberto a trocar ideia sobre Kafka, Clean Architecture ou o eterno debate de monólito vs. microsserviços.

</details>

---

## ⚙️ Stack

<div align="center">

**Backend**

<img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
<img alt="Spring Boot" src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" />
<img alt="Node.js" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
<img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />

**Mensageria &amp; Integração**

<img alt="Apache Kafka" src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white" />
<img alt="RabbitMQ" src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white" />
<img alt="REST e SOAP" src="https://img.shields.io/badge/REST%20%26%20SOAP-6E4AFF?style=for-the-badge&logo=swagger&logoColor=white" />

**Cloud &amp; DevOps**

<img alt="AWS" src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" />
<img alt="Azure DevOps" src="https://img.shields.io/badge/Azure%20DevOps-0078D7?style=for-the-badge&logo=azuredevops&logoColor=white" />
<img alt="Git" src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />

**Dados**

<img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
<img alt="MySQL" src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
<img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />

**Front-end &amp; Mobile**

<img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
<img alt="React" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
<img alt="Angular" src="https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white" />
<img alt="Flutter" src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" />

</div>

---

## 📌 Projetos em destaque

| Projeto | O que é | Stack |
| --- | --- | --- |
| [**clean-architeture-album**](https://github.com/kaiofelixdeoliveira/clean-architeture-album) ⭐ 11 | Referência prática de Clean Architecture em Java — separação de camadas, casos de uso e inversão de dependência. Meu repositório mais estrelado. | `Java` `Spring Boot` |
| [**kafka-producer**](https://github.com/kaiofelixdeoliveira/kafka-producer) · [**kafka-consumer**](https://github.com/kaiofelixdeoliveira/kafka-consumer) | Base de comunicação assíncrona com Apache Kafka: publicação e consumo de eventos prontos para reuso. | `Java` `Kafka` |
| [**rabbitmq-producer**](https://github.com/kaiofelixdeoliveira/rabbitmq-producer) · [**rabbitmq-consumer**](https://github.com/kaiofelixdeoliveira/rabbitmq-consumer) | Mesma ideia sobre AMQP: filas, consumidores e resiliência de mensagens com RabbitMQ. | `Java` `RabbitMQ` |
| [**azure-devops-pipeline**](https://github.com/kaiofelixdeoliveira/azure-devops-pipeline) | Pipeline de CI/CD no Azure DevOps para aplicações Java — build, testes e deploy automatizados. | `Azure DevOps` `Java` |
| [**projeto-contas**](https://github.com/kaiofelixdeoliveira/projeto-contas) | API de operações bancárias: consulta de saldo e transferência entre contas. | `Java` `Spring Boot` |
| [**stream-video-api**](https://github.com/kaiofelixdeoliveira/stream-video-api) · [**stream-video-app**](https://github.com/kaiofelixdeoliveira/stream-video-app) | API de streaming de vídeo com aplicativo mobile consumindo o serviço. | `Java` `Flutter` |
| [**starter-webservice-soap**](https://github.com/kaiofelixdeoliveira/starter-webservice-soap) | Ponto de partida para integração com web services SOAP — útil em cenários de legado. | `Java` `SOAP` |

<div align="center">
  <a href="https://github.com/kaiofelixdeoliveira?tab=repositories">
    <img alt="Ver todos os repositórios" src="https://img.shields.io/badge/Ver%20todos%20os%20reposit%C3%B3rios-0A66C2?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</div>

---

## 📊 Métricas

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=kaiofelixdeoliveira&show_icons=true&hide_border=true&include_all_commits=true&theme=tokyonight" />
  <img alt="Estatísticas do GitHub de Kaio Felix" src="https://github-readme-stats.vercel.app/api?username=kaiofelixdeoliveira&show_icons=true&hide_border=true&include_all_commits=true" height="165" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=kaiofelixdeoliveira&hide_border=true&theme=tokyonight" />
  <img alt="Sequência de contribuições de Kaio Felix" src="https://streak-stats.demolab.com?user=kaiofelixdeoliveira&hide_border=true" height="165" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=kaiofelixdeoliveira&layout=compact&langs_count=8&hide_border=true&theme=tokyonight" />
  <img alt="Linguagens mais usadas por Kaio Felix" src="https://github-readme-stats.vercel.app/api/top-langs/?username=kaiofelixdeoliveira&layout=compact&langs_count=8&hide_border=true" height="165" />
</picture>

<details>
<summary><b>📈 Ver gráfico de atividade</b></summary>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=kaiofelixdeoliveira&hide_border=true&theme=github-dark" />
  <img alt="Gráfico de atividade de Kaio Felix no GitHub" src="https://github-readme-activity-graph.vercel.app/graph?username=kaiofelixdeoliveira&hide_border=true&theme=github-compact" />
</picture>

</details>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/kaiofelixdeoliveira/kaiofelixdeoliveira/output/github-snake-dark.svg" />
  <img alt="Cobrinha percorrendo o gráfico de contribuições" src="https://raw.githubusercontent.com/kaiofelixdeoliveira/kaiofelixdeoliveira/output/github-snake.svg" />
</picture>

</div>

---

## 🤝 Vamos conversar

Aberto a trocas sobre **arquitetura de software, sistemas event-driven e liderança técnica** — e a oportunidades onde esses temas estejam no centro.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/Fale%20comigo%20no%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kaio-felix-oliveira/)
[![E-mail](https://img.shields.io/badge/kaio.felix.oliveira.mail%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kaio.felix.oliveira.mail@gmail.com)

</div>

---

<details>
<summary><b>🇺🇸 Read this profile in English</b></summary>

<br/>

### 👋 About me

I build — and lead the building of — **backend systems that have to stay up**: high volume, asynchronous integrations, and teams that change along the way. My bar isn't "works on my machine"; it's shipping software the next team can actually evolve.

<details>
<summary><b>🧑‍💼 I'm a manager or recruiter</b> — the 30-second version</summary>

<br/>

- 🏗️ **Architecture that supports the business** — Java/Spring Boot services built on Clean Architecture, keeping domain and infrastructure apart so swapping a database, a queue or a provider doesn't become a six-month project.
- 🔄 **Integrations that don't take the system down** — asynchronous messaging with Kafka and RabbitMQ: when a service fails, the queue absorbs it instead of the customer seeing an error.
- 🚀 **Predictable delivery** — CI/CD pipelines on Azure DevOps keep deployment off the team's critical path.
- 🧩 **End-to-end product** — when the team needs it, I go from the backend to the front-end (React, Angular) and mobile (Flutter).
- 🤝 **A stronger team than I found** — documented trade-offs, code review as part of delivery, and mentoring for junior developers.

Full career history on **[LinkedIn](https://www.linkedin.com/in/kaio-felix-oliveira/)**.

</details>

<details>
<summary><b>👨‍💻 I'm a developer or tech lead</b> — how I build software</summary>

<br/>

- **The domain doesn't know the framework.** If replacing Spring breaks a business rule, the design is wrong.
- **An event is a contract.** Payload changes are versioned, not "a quick fix in production".
- **Idempotency is not optional** in a queue consumer — reprocessing happens.
- **Legacy gets isolated, not cursed at.** An anti-corruption layer over SOAP, and the rest of the system keeps evolving.
- **Tests are executable documentation.** A use case without tests isn't done.

See it in code: [`clean-architeture-album`](https://github.com/kaiofelixdeoliveira/clean-architeture-album) · [`kafka-consumer`](https://github.com/kaiofelixdeoliveira/kafka-consumer) · [`starter-webservice-soap`](https://github.com/kaiofelixdeoliveira/starter-webservice-soap)

</details>

> 🔭 **Currently:** building a health and nutrition ecosystem (API, mobile app and web dashboard for professionals), using AI to support patient follow-up.

### ⚙️ Stack

`Java` · `Spring Boot` · `Node.js` · `Python` · `Kafka` · `RabbitMQ` · `REST & SOAP` · `AWS` · `Azure DevOps` · `PostgreSQL` · `MySQL` · `MongoDB` · `TypeScript` · `React` · `Angular` · `Flutter`

### 📌 Featured projects

| Project | What it is | Stack |
| --- | --- | --- |
| [**clean-architeture-album**](https://github.com/kaiofelixdeoliveira/clean-architeture-album) ⭐ 11 | A hands-on Clean Architecture reference in Java — layer separation, use cases and dependency inversion. My most starred repository. | `Java` `Spring Boot` |
| [**kafka-producer**](https://github.com/kaiofelixdeoliveira/kafka-producer) · [**kafka-consumer**](https://github.com/kaiofelixdeoliveira/kafka-consumer) | Reusable foundation for asynchronous communication with Apache Kafka. | `Java` `Kafka` |
| [**rabbitmq-producer**](https://github.com/kaiofelixdeoliveira/rabbitmq-producer) · [**rabbitmq-consumer**](https://github.com/kaiofelixdeoliveira/rabbitmq-consumer) | Same idea over AMQP: queues, consumers and message resilience. | `Java` `RabbitMQ` |
| [**azure-devops-pipeline**](https://github.com/kaiofelixdeoliveira/azure-devops-pipeline) | CI/CD pipeline on Azure DevOps for Java applications. | `Azure DevOps` `Java` |
| [**projeto-contas**](https://github.com/kaiofelixdeoliveira/projeto-contas) | Banking operations API: balance lookup and transfers between accounts. | `Java` `Spring Boot` |
| [**stream-video-api**](https://github.com/kaiofelixdeoliveira/stream-video-api) · [**stream-video-app**](https://github.com/kaiofelixdeoliveira/stream-video-app) | Video streaming API with a mobile app consuming the service. | `Java` `Flutter` |

### 🤝 Let's talk

Happy to discuss **software architecture, event-driven systems and technical leadership** — and open to opportunities where those are at the core.

[LinkedIn](https://www.linkedin.com/in/kaio-felix-oliveira/) · [kaio.felix.oliveira.mail@gmail.com](mailto:kaio.felix.oliveira.mail@gmail.com)

</details>

<img alt="" src="https://capsule-render.vercel.app/api?type=waving&color=0:6E4AFF,100:0A66C2&height=120&section=footer" />
