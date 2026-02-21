# Bet Engine: Sistema de Predicción y Gestión de Apuestas

Sistema distribuido diseñado para la predicción de resultados deportivos y optimización de capital mediante modelos de Machine Learning y gestión financiera avanzada. 

## Competiciones
- English Premier League

## Mercados
- 1x2.
- Over/Under 2.5 goles.
- Tarjetas.
- Tiros de esquina.

## Arquitectura del Sistema
El sistema se basa en una arquitectura de microservicios desacoplados para garantizar escalabilidad y mantenimiento:

- **Frontend:** React (Dashboard y señales).
- **Orquestador Backend:** Spring Boot (Java 21). Maneja la lógica de negocio, seguridad y gestión de Bankroll.
- **Motor de ML:** FastAPI (Python 3.12). Servicio de inferencia probabilística usando XGBoost.
- **Base de Datos:** PostgreSQL (Supabase) para almacenamiento de históricos y trazabilidad.



## Características Técnicas
- **Modelo:** Clasificación binaria con XGBoost optimizado por Log Loss.
- **Gestión de Riesgo:** Implementación de Kelly Fractional para el cálculo de Stake.
- **Shadow Tracking:** Monitoreo en tiempo real de la precisión del modelo vs resultados reales.
- **Infraestructura:** 100% Cloud-based (Vercel, Render, Supabase).