# Microservices - Ambiente Local com Docker Compose

Este repositório contém a configuração do **Docker Compose** para rodar localmente os serviços:  
- **Client Service**
- **Transaction Service**
- **API Gateway**  
Além dos bancos de dados, mensageria e cache necessários.

---

## 📂 Estrutura de Pastas

Para que o `docker-compose.yml` funcione corretamente, a **estrutura de diretórios** precisa ser:

```
/
├── docker-compose.yml
├── client-service/
│ ├── Dockerfile
│ └── ...
├── transaction-service/
│ ├── Dockerfile
│ └── ...
└── gateway/
├── Dockerfile
└── ..
```



> **Importante:** as pastas `client-service`, `transaction-service` e `gateway` devem estar no **mesmo nível** do arquivo `docker-compose.yml`.

---

## 🚀 Subindo o ambiente

1. **Clonar todos os repositórios** na mesma pasta (ou mover para a estrutura acima).
2. No terminal, na pasta onde está o `docker-compose.yml`, executar:

```bash
docker compose up --build
