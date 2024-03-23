# FIA PTPA2 - Professional Training and Pilot Advancement 2

<div align="center">

![FIA Logo](https://img.shields.io/badge/FIA-Professional%20Training-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**Sistema de Treinamento Profissional e Avanço de Piloto da FIA**

</div>

---

## 📋 Sobre o Projeto

O **FIA PTPA2** (Professional Training and Pilot Advancement 2) é um sistema completo desenvolvido para a **Federação Internacional de Automobilismo (FIA)** com o objetivo de gerenciar, acompanhar e promover o desenvolvimento profissional de pilotos em todas as categorias do automobilismo mundial.

Este sistema integrado permite o cadastro de pilotos, gestão de treinamentos, avaliação de desempenho, certificações, progressão de carreira e análise estatística de evolução técnica dos competidores.

### 🎯 Objetivos do Sistema FIA PTPA2

- **Gestão de Pilotos**: Cadastro completo de pilotos profissionais e aspirantes
- **Treinamentos**: Organização e acompanhamento de programas de capacitação
- **Certificações FIA**: Controle de licenças e certificações obrigatórias
- **Avaliação de Desempenho**: Métricas e análises de evolução técnica
- **Progressão de Carreira**: Acompanhamento da evolução entre categorias
- **Relatórios Gerenciais**: Dashboards e relatórios para tomada de decisão

---

## 🚀 Tecnologias Utilizadas

O sistema **FIA PTPA2** foi desenvolvido utilizando tecnologias modernas e robustas para garantir performance, escalabilidade e manutenibilidade:

### Backend

```
PHP 8.x com CodeIgniter 4
API RESTful
Arquitetura MVC
```

### Frontend

```
ReactJS 18.x
React Hooks
React Router
Axios para consumo de API
```

### Banco de Dados

```
MySQL 8.x
Modelagem Relacional
Stored Procedures
Triggers para auditoria
```

### Stack Completa

| Camada                     | Tecnologia     | Versão |
| -------------------------- | -------------- | ------ |
| **Backend**                | PHP            | 8.x    |
| **Framework Backend**      | CodeIgniter    | 4.x    |
| **API**                    | RESTful        | -      |
| **Frontend**               | ReactJS        | 18.x   |
| **Banco de Dados**         | MySQL          | 8.x    |
| **Servidor Web**           | Apache/Nginx   | 2.4+   |
| **Gerenciador de Pacotes** | Composer / NPM | Latest |

---

## 📊 Métricas de Desenvolvimento

### Análise de Pontos de Função (APF)

O projeto **FIA PTPA2** utiliza a metodologia de **Pontos de Função** como métrica principal para estimar o esforço de desenvolvimento, complexidade e custo do sistema.

#### Contagem de Pontos de Função - FIA PTPA2

| Tipo de Função                       | Complexidade | Quantidade | PF Unitário | PF Total |
| ------------------------------------ | ------------ | ---------- | ----------- | -------- |
| **Entradas Externas (EI)**           | Baixa        | 12         | 3           | 36       |
|                                      | Média        | 18         | 4           | 72       |
|                                      | Alta         | 8          | 6           | 48       |
| **Saídas Externas (EO)**             | Baixa        | 10         | 4           | 40       |
|                                      | Média        | 15         | 5           | 75       |
|                                      | Alta         | 6          | 7           | 42       |
| **Consultas Externas (EQ)**          | Baixa        | 14         | 3           | 42       |
|                                      | Média        | 12         | 4           | 48       |
|                                      | Alta         | 5          | 6           | 30       |
| **Arquivos Lógicos Internos (ALI)**  | Baixa        | 8          | 7           | 56       |
|                                      | Média        | 10         | 10          | 100      |
|                                      | Alta         | 4          | 15          | 60       |
| **Arquivos Interface Externa (AIE)** | Baixa        | 3          | 5           | 15       |
|                                      | Média        | 5          | 7           | 35       |
|                                      | Alta         | 2          | 10          | 20       |

**Total de Pontos de Função Não Ajustados:** **719 PF**

#### Fatores de Ajuste

| Fator                       | Peso | Descrição                           |
| --------------------------- | ---- | ----------------------------------- |
| Comunicação de Dados        | 4    | Sistema integrado com APIs externas |
| Processamento Distribuído   | 3    | Backend e Frontend separados        |
| Performance                 | 5    | Alta performance requerida          |
| Configuração Complexa       | 3    | Múltiplos perfis e configurações    |
| Volume de Transações        | 4    | Alto volume de operações            |
| Entrada de Dados Online     | 5    | Sistema web interativo              |
| Eficiência do Usuário Final | 4    | Interface amigável e responsiva     |
| Atualização Online          | 5    | Atualizações em tempo real          |
| Processamento Complexo      | 4    | Cálculos e validações complexas     |
| Reusabilidade               | 3    | Componentes reutilizáveis           |
| Facilidade de Instalação    | 3    | Docker e ambiente configurável      |
| Facilidade de Operação      | 4    | Interface administrativa completa   |
| Múltiplos Sites             | 2    | Deploy em diferentes ambientes      |
| Facilidade de Mudanças      | 4    | Arquitetura modular                 |

**Fator de Ajuste Total:** 53  
**Influência:** 0.65 + (0.01 × 53) = **1.18**

**Pontos de Função Ajustados:** 719 × 1.18 = **848 PF**

#### Estimativa de Esforço

Considerando a produtividade média de **10 PF/homem-mês** para sistemas de alta complexidade:

- **Esforço Total Estimado:** 848 PF ÷ 10 = **84.8 homens-mês**
- **Duração Estimada:** 12 meses (equipe de 7 desenvolvedores)
- **Custo Estimado:** Variável conforme região e senioridade da equipe

---

## 🏗️ Arquitetura do Sistema FIA PTPA2

### Estrutura de Diretórios

```
fiaptpa2-main/
├── backend/                    # API REST em CodeIgniter
│   ├── app/
│   │   ├── Controllers/       # Controladores da API
│   │   ├── Models/            # Modelos de dados
│   │   ├── Database/          # Migrations e Seeds
│   │   ├── Filters/           # Autenticação e autorização
│   │   ├── Libraries/         # Bibliotecas customizadas
│   │   └── Config/            # Configurações
│   ├── public/                # Ponto de entrada
│   ├── writable/              # Logs e cache
│   └── tests/                 # Testes automatizados
│
├── frontend/                   # Interface em ReactJS
│   ├── public/                # Arquivos estáticos
│   ├── src/
│   │   ├── components/        # Componentes reutilizáveis
│   │   ├── pages/             # Páginas da aplicação
│   │   ├── services/          # Consumo de API
│   │   ├── contexts/          # Context API
│   │   ├── hooks/             # Custom Hooks
│   │   ├── utils/             # Funções auxiliares
│   │   └── assets/            # Imagens e estilos
│   ├── package.json
│   └── vite.config.js
│
├── database/                   # Scripts SQL
│   ├── schema/                # Estrutura do banco
│   ├── migrations/            # Migrações
│   ├── seeds/                 # Dados iniciais
│   └── procedures/            # Stored Procedures
│
├── docs/                       # Documentação
│   ├── api/                   # Documentação da API
│   ├── database/              # Modelagem do banco
│   ├── requisitos/            # Especificação de requisitos
│   └── manuais/               # Manuais de usuário
│
├── docker/                     # Containers Docker
│   ├── docker-compose.yml
│   ├── Dockerfile.backend
│   └── Dockerfile.frontend
│
├── .env.example               # Exemplo de variáveis de ambiente
├── .gitignore
├── LICENSE
└── README.md
```

---

## 🎨 Funcionalidades Principais do FIA PTPA2

### 1. Gestão de Pilotos

- ✅ Cadastro completo de pilotos (dados pessoais, nacionalidade, categoria)
- ✅ Histórico de competições e resultados
- ✅ Documentação digital (licenças, certificados médicos)
- ✅ Gestão de patrocinadores e equipes

### 2. Programa de Treinamento FIA

- ✅ Cadastro de cursos e módulos de capacitação
- ✅ Agendamento de treinamentos presenciais e online
- ✅ Acompanhamento de progresso e conclusão
- ✅ Avaliações teóricas e práticas
- ✅ Emissão de certificados digitais FIA

### 3. Sistema de Certificação

- ✅ Controle de licenças Super License
- ✅ Requisitos por categoria (F1, F2, F3, Formula E, etc.)
- ✅ Renovação automática e alertas de vencimento
- ✅ Histórico de certificações

### 4. Avaliação de Desempenho

- ✅ Métricas de performance em pista
- ✅ Avaliação de instrutores FIA
- ✅ Análise comparativa entre pilotos
- ✅ Relatórios de evolução técnica

### 5. Progressão de Carreira

- ✅ Acompanhamento da evolução entre categorias
- ✅ Requisitos para avanço (pontos, certificações, experiência)
- ✅ Recomendações personalizadas de treinamento
- ✅ Pipeline de talentos FIA

### 6. Dashboard e Relatórios

- ✅ Painel administrativo FIA
- ✅ Estatísticas gerais de pilotos ativos
- ✅ Relatórios de certificações emitidas
- ✅ Análise de efetividade dos treinamentos
- ✅ Exportação de dados (PDF, Excel, CSV)

### 7. Integração com Sistemas FIA

- ✅ API para integração com calendário de provas
- ✅ Sincronização com resultados de competições
- ✅ Importação de dados de telemetria
- ✅ Webhook para notificações em tempo real

---

## ⚙️ Instalação e Configuração

### Pré-requisitos

- **PHP** >= 8.0
- **Composer** >= 2.0
- **Node.js** >= 18.0
- **MySQL** >= 8.0
- **Apache/Nginx**
- **Git**

### 1️⃣ Clonar o Repositório

```bash
git clone https://github.com/fia/fiaptpa2-main.git
cd fiaptpa2-main
```

### 2️⃣ Configurar Backend (CodeIgniter)

```bash
cd backend
composer install
cp .env.example .env
# Edite o arquivo .env com suas configurações de banco de dados
php spark migrate
php spark db:seed
php spark serve
```

### 3️⃣ Configurar Frontend (ReactJS)

```bash
cd frontend
npm install
cp .env.example .env
# Configure a URL da API no .env
npm run dev
```

### 4️⃣ Configurar Banco de Dados

```bash
# Importar schema inicial
mysql -u root -p fia_ptpa2 < database/schema/initial_schema.sql

# Executar seeds de dados iniciais
mysql -u root -p fia_ptpa2 < database/seeds/inicial_data.sql
```

### 5️⃣ Docker (Opcional)

```bash
docker-compose up -d
```

---

## 🔑 Variáveis de Ambiente

### Backend (.env)

```env
CI_ENVIRONMENT = development
app.baseURL = 'http://localhost:8080'

database.default.hostname = localhost
database.default.database = fia_ptpa2
database.default.username = root
database.default.password =
database.default.DBDriver = MySQLi

JWT_SECRET_KEY = your-secret-key-here
JWT_TIME_TO_LIVE = 3600
```

### Frontend (.env)

```env
VITE_API_URL=http://localhost:8080/api
VITE_APP_NAME=FIA PTPA2
VITE_APP_VERSION=2.0.0
```

---

## 🗄️ Modelagem de Dados - FIA PTPA2

### Principais Entidades

```
- Pilotos (drivers)
- Categorias (categories)
- Licenças (licenses)
- Treinamentos (trainings)
- Módulos de Curso (training_modules)
- Matrículas (enrollments)
- Avaliações (assessments)
- Certificados (certificates)
- Competições (competitions)
- Resultados (results)
- Equipes (teams)
- Instrutores (instructors)
- Auditoria (audit_logs)
```

### Diagrama ER (Resumido)

```
Pilotos 1---N Licenças
Pilotos 1---N Matrículas
Pilotos 1---N Resultados
Treinamentos 1---N Módulos
Treinamentos 1---N Matrículas
Matrículas 1---N Avaliações
Matrículas 1---1 Certificados
Equipes 1---N Pilotos
Competições 1---N Resultados
```

---

## 🔐 Autenticação e Segurança

O **FIA PTPA2** implementa múltiplas camadas de segurança:

- ✅ **JWT (JSON Web Token)** para autenticação de API
- ✅ **CORS** configurado adequadamente
- ✅ **Rate Limiting** para prevenir abusos
- ✅ **SQL Injection** prevenção com Prepared Statements
- ✅ **XSS Protection** com sanitização de dados
- ✅ **HTTPS** obrigatório em produção
- ✅ **Logs de Auditoria** para todas operações críticas
- ✅ **Controle de Acesso** baseado em roles (Admin, Instrutor, Piloto)

---

## 🧪 Testes

### Backend

```bash
cd backend
composer test
```

### Frontend

```bash
cd frontend
npm run test
```

### Cobertura de Testes

- **Backend:** > 80% de cobertura
- **Frontend:** > 75% de cobertura

---

## 📱 API Endpoints (Resumo)

### Autenticação

```
POST   /api/auth/login
POST   /api/auth/register
POST   /api/auth/refresh
POST   /api/auth/logout
```

### Pilotos

```
GET    /api/pilots
GET    /api/pilots/{id}
POST   /api/pilots
PUT    /api/pilots/{id}
DELETE /api/pilots/{id}
```

### Treinamentos

```
GET    /api/trainings
GET    /api/trainings/{id}
POST   /api/trainings
PUT    /api/trainings/{id}
DELETE /api/trainings/{id}
POST   /api/trainings/{id}/enroll
```

### Certificações

```
GET    /api/certificates
GET    /api/certificates/{id}
POST   /api/certificates
GET    /api/certificates/pilot/{pilotId}
```

**Documentação Completa:** `/docs/api/swagger.json`

---

## 👥 Perfis de Usuário

| Perfil                | Permissões                              |
| --------------------- | --------------------------------------- |
| **Administrador FIA** | Acesso total ao sistema                 |
| **Instrutor**         | Gerenciar treinamentos, avaliar pilotos |
| **Piloto**            | Visualizar dados pessoais, fazer cursos |
| **Gestor de Equipe**  | Visualizar pilotos da equipe            |
| **Auditor**           | Acesso somente leitura aos logs         |

---

## 📈 Roadmap do FIA PTPA2

### Versão 2.0 (Atual)

- [x] Sistema base de gestão de pilotos
- [x] Módulo de treinamentos
- [x] Sistema de certificação
- [x] Dashboard administrativo

### Versão 2.1 (Próxima)

- [ ] Integração com telemetria em tempo real
- [ ] App mobile (iOS/Android)
- [ ] Sistema de gamificação
- [ ] IA para recomendação de treinamentos

### Versão 2.2 (Futuro)

- [ ] Realidade Virtual para treinamentos
- [ ] Blockchain para certificados
- [ ] Análise preditiva de desempenho
- [ ] Marketplace de instrutores

---

## 🤝 Contribuindo

Contribuições são sempre bem-vindas! Para contribuir com o **FIA PTPA2**:

1. Faça um Fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

### Padrões de Código

- **PHP:** PSR-12
- **JavaScript:** Airbnb Style Guide
- **Commits:** Conventional Commits

---

## 📞 Suporte

Para questões sobre o **FIA PTPA2**, entre em contato:

- **Email:** ptpa2@fia.com
- **Issue Tracker:** [GitHub Issues](https://github.com/fia/fiaptpa2-main/issues)
- **Wiki:** [Documentação Técnica](https://github.com/fia/fiaptpa2-main/wiki)

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 👨‍💻 Equipe de Desenvolvimento

Desenvolvido com ❤️ pela equipe de tecnologia da **FIA** (Federação Internacional de Automobilismo)

---

<div align="center">

### FIA PTPA2 - Elevando o Padrão do Automobilismo Mundial 🏎️

**Professional Training and Pilot Advancement 2**

[![FIA](https://img.shields.io/badge/FIA-Official%20System-red?style=flat-square)](https://www.fia.com)
[![CodeIgniter](https://img.shields.io/badge/CodeIgniter-4.x-orange?style=flat-square)](https://codeigniter.com)
[![React](https://img.shields.io/badge/React-18.x-blue?style=flat-square)](https://reactjs.org)
[![MySQL](https://img.shields.io/badge/MySQL-8.x-blue?style=flat-square)](https://www.mysql.com)

</div>
