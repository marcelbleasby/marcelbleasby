<h1 align="center">Marcel Bastos Bleasby</h1>

<p align="center">
  <b>Backend & Platform Engineer</b> · Ciência da Computação — UFC Russas<br>
  Construindo plataformas multi-tenant em saúde, telecom e foodservice na <a href="https://github.com/B-M-O-Be-More">@B-M-O-Be-More</a>
</p>

<p align="center">
  <a href="https://github.com/marcelbleasby"><img src="https://img.shields.io/badge/GitHub-marcelbleasby-181717?style=flat-square&logo=github" alt="GitHub"></a>
  <a href="mailto:marcelbleasby@bmo.dev.br"><img src="https://img.shields.io/badge/Email-marcelbleasby@bmo.dev.br-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Russas-CE,%20Brasil-0A66C2?style=flat-square&logo=googlemaps&logoColor=white" alt="Localização">
</p>

---

## Sobre

Desenvolvo sistemas de ponta a ponta: da API multi-tenant ao firmware que lê o cartão no balcão.
Meu foco é **backend Python** (Django e FastAPI) com arquitetura modular, controle de acesso granular e operação em Docker — mas os projetos costumam atravessar camadas: frontend Next.js, serviço Windows em .NET, app Android/Wear OS em Kotlin e firmware STM32 em C.

Domínios em que tenho entregado: **imagem médica (PACS/DICOM)**, **gestão de cozinhas industriais**, **infraestrutura óptica/GIS**, **pagamentos e identidade** e **segurança de rede**.

---

## Stack

**Backend**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![DRF](https://img.shields.io/badge/Django%20REST-A30000?style=flat-square&logo=django&logoColor=white)
![Django Ninja](https://img.shields.io/badge/Django%20Ninja-4CAF50?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)

**Frontend & Mobile**
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![MUI](https://img.shields.io/badge/MUI-007FFF?style=flat-square&logo=mui&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)
![Wear OS](https://img.shields.io/badge/Wear%20OS-4285F4?style=flat-square&logo=wearos&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0071E3?style=flat-square&logo=swift&logoColor=white)

**Dados & Infra**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![PostGIS](https://img.shields.io/badge/PostGIS-336791?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![MinIO](https://img.shields.io/badge/S3%20%2F%20MinIO-C72E49?style=flat-square&logo=minio&logoColor=white)

**Sistemas & Embarcados**
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![NFC](https://img.shields.io/badge/NFC%20%2F%20ISO14443A-0F62FE?style=flat-square)

---

## Competências

### Arquitetura de plataformas multi-tenant
Isolamento lógico estrito por empresa com estreitamento contextual por unidade, RBAC granular baseado em slugs (`recurso.acao.escopo`) com hierarquia de escopo e cache em Redis, planos e tetos de permissão por assinatura, e webhooks de pagamento autenticados via HMAC-SHA256.

### APIs assíncronas e tempo real
Django 5 + Django Ninja Extra sobre ASGI/Uvicorn, FastAPI com SQLAlchemy async e Alembic, WebSockets (Channels) para eventos de terminais, Celery para tarefas periódicas e assíncronas.

### Segurança aplicada
Autenticação JWT, 2FA para administradores, correção de escalonamento de privilégio, tokens de dispositivo (`X-Terminal-Token`), validação mágica de bytes em upload, `auth_request` no Nginx, TLS 1.2/1.3, assinatura digital de documentos com certificado A1, roles de banco sem superuser e `audit_log` imutável com retenção programada.

### Auditoria e rastreabilidade
Logs estruturados por usuário com soft delete, retenção, estatísticas e exportação CSV; fluxo de conferência cega de estoque com congelamento de snapshot, cálculo de divergência e tolerâncias configuráveis.

### Integração com hardware (NFC / embarcados)
Firmware STM32F411 + PN532 enumerando como **leitor USB CCID** padrão (sem driver no Windows), serviço Windows em .NET 6 com PCSC e motor de sincronização offline, desktop Python de gravação de cartões, emulação **HCE** em Android e análise de cartões com Proxmark3.

### Mobile — Android e iOS
Apps Android em **Kotlin com Jetpack Compose**: Material 3, navegação e ViewModel em Compose, injeção de dependência com Hilt e consumo de API com Retrofit. Extensão para **Wear OS** com Compose, serviços wearable e interações remotas com o celular. Em **iOS/Swift**, experiência básica focada em construção de interface.

### Imagem médica — PACS/DICOM
Stack white label com Orthanc, DICOMweb (QIDO-RS/WADO-RS), viewer Cornerstone3D, servidor de **Modality Worklist** nativo em FastAPI com `pynetdicom`, laudo estruturado com templates e geração de PDF (WeasyPrint isolado em subprocesso), portal do paciente e separação de papéis médico/recepção/admin sob LGPD.

### Geoespacial e ML aplicado
Pipeline que reconstrói infraestrutura óptica a partir de KML/KMZ: ingestão GIS, análise geoespacial por autômato, normalização semântica e orquestração cognitiva por confiança, com ontologia compartilhada, PostGIS e WGS84 ponta a ponta.

### Dados e BI
Datasets analíticos em Apache Parquet no S3/MinIO com URLs assinadas para consumo em Metabase/Superset/Power BI, dashboards operacionais e motor dinâmico de relatórios PDF/CSV que adapta a paleta à identidade visual do cliente.

### Engenharia de software
Monorepos orquestrados por Docker Compose, migrations com Alembic, testes com pytest, revisão de código e trabalho em PRs com worktrees, documentação técnica (SDD, ADR, glossário) e automação com Claude Code.

---

## Projetos

| Projeto | O que é | Stack |
| --- | --- | --- |
| **[orthanc-stack](https://github.com/marcelbleasby/orthanc-stack)** | PACS/DICOM white label: armazenamento, viewer e laudo, com MWL nativo e portal do paciente | FastAPI · React · Orthanc · PostgreSQL · Nginx |
| **Mennu** | Plataforma multi-tenant para cozinhas industriais: cardápios, estoque por lote, auditoria cega, terminais NFC e BI | Django Ninja · Next.js · .NET · Celery · Redis |
| **Neutramais** | Backend de infraestrutura de telecomunicações com CTOs, ordens de serviço e dados geoespaciais | Django · DRF · PostGIS · Celery |
| **[Class_KML_KMZ](https://github.com/marcelbleasby/Class_KML_KMZ)** | Motor semântico-topológico que reconstrói infraestrutura óptica a partir de KML/KMZ | Python · scikit-learn · XGBoost · PostGIS |
| **[edge-security](https://github.com/marcelbleasby/edge-security)** | Monitoramento passivo de rede e administração DNS | Suricata · Pi-hole · FastAPI · Next.js |
| **[RU_Virtual](https://github.com/marcelbleasby/RU_Virtual)** | App de restaurante universitário com emulação de cartão via HCE e versão Wear OS | Kotlin · Jetpack Compose · Hilt · Retrofit · Wear OS |
| **firmware-nfc-reader** | Leitor NFC USB CCID em STM32F411 + PN532 | C · STM32 · SPI · USB OTG |

---

## GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=marcelbleasby&show_icons=true&hide_border=true&count_private=true&include_all_commits=true&theme=github_dark" alt="Estatísticas do GitHub">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=marcelbleasby&layout=compact&hide_border=true&langs_count=8&theme=github_dark" alt="Linguagens mais usadas">
</p>

---

<p align="center">
  <i>Aberto a conversas sobre backend, imagem médica e sistemas que encostam em hardware.</i>
</p>
