# 🏥 Voll.med API

API REST desenvolvida em **Java com Spring Boot**, baseada no projeto do curso da **Alura**, para o gerenciamento de médicos, pacientes e consultas de uma clínica fictícia.  
O objetivo é aplicar boas práticas de arquitetura, validação, persistência e versionamento de APIs modernas.

---

## 📋 Sumário
- [Sobre o projeto](#sobre-o-projeto)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
- [Estrutura do projeto](#estrutura-do-projeto)
- [Como executar o projeto](#como-executar-o-projeto)
- [Endpoints principais](#endpoints-principais)
- [Boas práticas aplicadas](#boas-práticas-aplicadas)
- [Autor](#autor)

---

## 🧠 Sobre o projeto

O **Voll.med API** simula o sistema de uma clínica médica, permitindo o **cadastro, listagem, atualização e exclusão** de médicos e pacientes, além do **agendamento de consultas**.

O projeto segue o padrão **MVC (Model-View-Controller)** e aplica conceitos de **boas práticas de API REST**, **validação com Bean Validation**, **mapeamento JPA**, **autenticação JWT**, e **documentação com Swagger**.

---

## 🚀 Tecnologias utilizadas

| Categoria | Tecnologias |
|------------|--------------|
| Linguagem | Java 17+ |
| Framework principal | Spring Boot 3+ |
| Banco de dados | MySQL |
| ORM | Hibernate / JPA |
| Segurança | Spring Security + JWT |
| Migrações | Flyway |
| Documentação | SpringDoc / Swagger UI |
| Build | Maven |
| Testes | JUnit / Mockito |
| Deploy | Vercel (frontend) + Docker (opcional) |

---

## 🧩 Estrutura do projeto

src/
├── main/
│ ├── java/med/voll/api/
│ │ ├── controller/ # Controladores REST
│ │ ├── domain/ # Entidades e regras de negócio
│ │ ├── repository/ # Interfaces JPA
│ │ └── service/ # Lógica de aplicação (se houver)
│ └── resources/
│ ├── application.properties # Configurações
│ └── db/migration/ # Scripts Flyway
└── test/
└── ... # Testes automatizados



---

## ⚙️ Como executar o projeto

### 🧾 Pré-requisitos
- Java 17+
- Maven 3.8+
- MySQL (rodando localmente)

### 💡 Passos

1. Clone o repositório:
   ```bash
   git clone https://github.com/MathReis97/Voll.med-API.git
📡 Endpoints principais
Método	Endpoint	Descrição
POST	/medicos	Cadastrar novo médico
GET	/medicos	Listar médicos
PUT	/medicos	Atualizar informações
DELETE	/medicos/{id}	Excluir médico
POST	/pacientes	Cadastrar paciente
GET	/pacientes	Listar pacientes
POST	/consultas	Agendar consulta
DELETE	/consultas/{id}	Cancelar consulta

🔐 Alguns endpoints exigem autenticação JWT.

👨‍💻 Autor

Matheus Reis
📧 https://www.linkedin.com/in/matheusrd-reis/
💼 https://github.com/MathReis97
