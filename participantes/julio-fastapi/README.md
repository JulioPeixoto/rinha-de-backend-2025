# Rinha de Backend 2025 - FastAPI + Redis + Nginx

## Tecnologias Utilizadas

- **FastAPI** - Framework web moderno e rápido
- **Redis** - Cache e armazenamento de dados
- **Nginx** - Load balancer
- **Docker** - Containerização
- **Uvicorn + Uvloop** - Servidor ASGI de alta performance

## Estratégia

- Load balancer Nginx com 2 instâncias FastAPI
- Fallback automático entre processadores default/fallback
- Cache Redis para consistência de dados
- Timeouts otimizados para reduzir latência

## Recursos

- **CPU**: 1.5 total (0.15 nginx + 0.60 api1 + 0.60 api2 + 0.15 redis)
- **Memória**: 350MB total (30MB nginx + 130MB api1 + 130MB api2 + 40MB redis)

## Repositório

https://github.com/juliopeixoto/rinha-fastapi