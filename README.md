#  PlantIA API

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white"/>
  <img src="https://img.shields.io/badge/REST_API-005571?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/IoT-00B4D8?style=for-the-badge&logo=raspberrypi&logoColor=white"/>
</p>

API REST desenvolvida em Flask como parte do **Sistema de Irrigação Inteligente com IA**. Responsável por expor os dados de irrigação e os diagnósticos de saúde das plantas - gerados por inteligência artificial via análise de imagens — para consumo pelo aplicativo mobile do sistema.

>  Este repositório faz parte do projeto maior [**Smart Irrigation System**](https://github.com/Thiiagoramos/PlantIA).

---

##  Funcionalidades

-  Endpoints REST para consulta de dados de irrigação
-  Retorno de diagnósticos gerados por IA (análise de imagens de plantas)
-  Integração com aplicativo mobile para visualização em tempo real
-  Deploy configurado via `Procfile` (compatível com Heroku/Railway)

---

##  Onde esta API se encaixa

```
[Sensor de Solo / Câmera]
         ↓
 [IA — diagnóstico por imagem]
         ↓
    [Banco de Dados]
         ↓
   [PlantIA API]  ←────────→  [App Mobile]
```

---

##  Estrutura do Projeto

```
PlantIA-api/
├── app.py            # Aplicação Flask e definição das rotas
├── requirements.txt  # Dependências do projeto
├── Procfile          # Configuração de deploy
└── .gitignore
```

---

##  Como Executar Localmente

1. Clone o repositório:
```bash
git clone https://github.com/Thiiagoramos/PlantIA-api.git
cd PlantIA-api
```

2. Crie e ative um ambiente virtual:
```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

3. Instale as dependências:
```bash
pip install -r requirements.txt
```

4. Execute a aplicação:
```bash
python app.py
```

A API estará disponível em `http://localhost:5000`.

---

##  Dependências

Listadas em `requirements.txt`. As principais incluem:
- `Flask` - framework web
- `flask-cors` - suporte a CORS para consumo pelo app mobile

---

##  Próximas melhorias

- [ ] Documentar endpoints com Swagger / OpenAPI
- [ ] Adicionar autenticação via JWT
- [ ] Adicionar testes automatizados
- [ ] Migrar para FastAPI para melhor performance

---

## 🔗 Repositórios do Projeto

| Repositório | Descrição |
|------------|-----------|
| [PlantIA](https://github.com/Thiiagoramos/PlantIA) | Visão geral e arquitetura do projeto completo |
| [PlantIA-api](https://github.com/Thiiagoramos/PlantIA-api) | Esta API - back-end Flask |
| *(App Mobile)* | Aplicativo de visualização dos dados |
| *(IA / Diagnóstico)* | Módulo de análise de imagens |

---

## 👤 Autor

**Thiago Ramos** — [LinkedIn](https://www.linkedin.com/in/thiago-ramos-a86107279)
