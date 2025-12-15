# Hallazgos — Sistema de gestión institucional (Hub)

Este documento resume los principales hallazgos detectados durante el proceso
de testing y auditoría funcional del sistema.

Los hallazgos se presentan de forma tipificada y abstracta, sin exponer datos
reales ni información sensible.

---

## 1. Falta de feedback en acciones críticas
**Descripción:**  
El sistema no informa de manera clara si una acción fue realizada con éxito
(alta, edición, cambio de estado).

**Impacto:**  
Puede generar duplicaciones, errores operativos y retrabajo administrativo.

**Observación QA:**  
La ausencia de feedback obliga al usuario a inferir el estado del sistema.

---

## 2. Validaciones insuficientes en cargas de datos
**Descripción:**  
Se detecta dificultad para cargar datos reales o no normalizados provenientes
de fuentes externas (por ejemplo, planillas).

**Impacto:**  
Imposibilita el uso directo de datos existentes y complica la adopción del sistema.

**Observación QA:**  
El sistema parece asumir un modelo de datos ideal no explicitado.

---

## 3. Persistencia de estados sin indicación visible
**Descripción:**  
Búsquedas o filtros aplicados persisten sin señalización clara para el usuario.

**Impacto:**  
Confusión en la lectura de resultados y posibles interpretaciones erróneas.

**Observación QA:**  
La interfaz no acompaña la memoria del estado del sistema.

---

## 4. Barreras de accesibilidad en formularios
**Descripción:**  
Campos obligatorios, mensajes de error y estados no presentan indicaciones
accesibles ni consistentes.

**Impacto:**  
Dificulta o imposibilita el uso por personas que utilizan tecnologías asistivas.

**Observación QA:**  
La accesibilidad no parece integrada como criterio de diseño.

---

## 5. Terminología técnica sin apoyo contextual
**Descripción:**  
Se utilizan términos técnicos o administrativos sin ayuda, glosario o referencia.

**Impacto:**  
Curva de aprendizaje elevada y dependencia de conocimiento previo.

**Observación QA:**  
El sistema asume un usuario experto sin ofrecer acompañamiento.

---

## Nota final
Los hallazgos aquí descriptos representan patrones observados durante el testing
y no constituyen un listado exhaustivo de incidencias.
