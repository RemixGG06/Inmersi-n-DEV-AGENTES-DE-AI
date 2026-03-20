# INMERSION-DEV-AGENTES-DE-AI
Sistema de agente inteligente capaz de decidir dinámicamente entre consultar documentos internos (RAG) o información en la web, generando respuestas estructuradas y exportables.
## 🚀 Descripción

Este proyecto implementa un **agente de IA basado en arquitectura híbrida (RAG + Web Search)** que:

- Analiza preguntas del usuario
- Decide automáticamente la mejor fuente de información:
  - 📄 Documentos internos (PDFs)
  - 🌐 Web (búsqueda en tiempo real)
- Genera respuestas estructuradas en formato Markdown
- Permite exportar resultados a PDF

El sistema simula el comportamiento de asistentes inteligentes modernos utilizados en entornos empresariales.
## 🧠 Arquitectura del Sistema
El flujo del agente está basado en un grafo de estados:
Usuario → Clasificación → (RAG | Web) → Contexto → LLM → Respuesta estructurada
🔹 Componentes principales:

- **Router (Decision Node):**
  Determina si la consulta debe resolverse con RAG o Web

- **RAG Pipeline:**
  - Carga de PDFs
  - Fragmentación (chunking)
  - Embeddings
  - Búsqueda semántica (FAISS)

- **Web Search:**
  - Integración con SerpAPI para consultas en tiempo real

- **LLM (Gemini):**
  - Generación de respuestas estructuradas
  - Formato en Markdown
  
## 🛠️ Stack Tecnológico
- **Lenguaje:** Python  
- **LLM:** Gemini 2.5 Flash  
- **Framework:** LangChain + LangGraph  
- **Embeddings:** `gemini-embedding-001`  
- **Vector Store:** FAISS  
- **Web Search:** SerpAPI  
- **PDF Processing:** PyPDF  
- **Exportación:** ReportLab  
---

## 🔍 Funcionalidades

✅ Clasificación automática de consultas (RAG vs Web)  
✅ Búsqueda semántica en documentos  
✅ Integración con datos en tiempo real  
✅ Generación de respuestas estructuradas  
✅ Exportación automática a PDF  
✅ Arquitectura modular basada en nodos  

--- 

Este proyecto demuestra:
Diseño de agentes IA
Orquestación de herramientas (RAG + Web)
Optimización de llamadas a LLM
Generación de contenido estructurado
Construcción de sistemas aplicables a negocio
--- 
--- 
Mejoras Futuras

Interfaz tipo chatbot (Streamlit / Web)
Memoria conversacional
Soporte multi-documento avanzado
Deploy en la nube (Render / GCP)
Exportación a Word (.docx)
Integración con bases de datos
--- 

##Desarrollado por ALVARO MONCADA 

💡 Enfocado en Inteligencia Artificial aplicada, automatización y sistemas inteligentes.
