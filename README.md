# PoC – Abuso de Configuraciones Predeterminadas en Vertex AI  
**CVE-2023-43654 / GCP-2023-029 (Contexto Vertex AI)**

## ⚠️ Aviso Importante
Este repositorio contiene una **Prueba de Concepto (PoC) educativa y defensiva**.  
**NO incluye exploits funcionales**, ejecución remota de código real, robo de credenciales ni abuso activo de servicios en la nube.  
Su objetivo es **demostrar el riesgo**, **validar configuraciones inseguras** y **apoyar tareas de detección y mitigación**.

---

## 📌 Resumen
Investigaciones recientes han demostrado que ciertas **configuraciones predeterminadas en Vertex AI** pueden permitir que usuarios con **bajos privilegios** accedan indirectamente a **roles de agentes de servicio** con permisos amplios.  
En escenarios específicos, esto puede derivar en **escalamiento de privilegios**, **acceso a recursos sensibles** y **ejecución de código no autorizada**, especialmente cuando se combinan con vulnerabilidades conocidas como **CVE-2023-43654 en TorchServe**.

Esta PoC documenta y simula estos flujos de riesgo sin explotarlos activamente.

---

## 🎯 Objetivos de la PoC
- Documentar el **flujo de abuso de permisos** en Vertex AI  
- Simular el impacto del **acceso indebido a agentes de servicio**  
- Identificar **configuraciones inseguras** en:
  - Vertex AI Agent Engine  
  - Ray on Vertex AI  
  - TorchServe (contexto CVE-2023-43654)  
- Proveer **scripts de auditoría y detección**  
- Facilitar la **validación de mitigaciones**

---

## 🧩 Alcance
Incluye:
- Análisis conceptual del vector de ataque  
- Scripts **read-only** de auditoría  
- Payloads simulados (no ejecutables)  
- Ejemplos de configuraciones seguras vs inseguras  
- Evidencia y resultados esperados  
- Exploits funcionales  
