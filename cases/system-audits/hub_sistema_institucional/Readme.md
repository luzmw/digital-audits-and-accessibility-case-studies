# Caso de estudio — Sistema de gestión institucional (Hub)

## Contexto general
Este caso documenta un proceso de auditoría y testing sobre un sistema institucional
de gestión de aplicaciones y servidores, utilizado en un organismo público.

El sistema permite el alta, edición, consulta y administración de registros técnicos,
con flujos administrativos internos y sin documentación funcional formal.

## Objetivo del análisis
- Evaluar la capacidad del sistema para operar con datos reales.
- Detectar inconsistencias funcionales, de usabilidad y accesibilidad.
- Analizar riesgos operativos derivados de la falta de feedback y validaciones.
- Documentar el proceso de testing en contextos con baja o nula documentación.

## Enfoque y metodología
- Testing manual y exploratorio.
- Análisis de flujos “felices” y alternativos.
- Evaluación de usabilidad y accesibilidad básica.
- Registro de hallazgos a partir de evidencia observable.
- Uso de datos anonimizados y ejemplos ficticios.

- ## Workflow aplicado en el análisis (versión pública)

El siguiente workflow describe el enfoque general utilizado durante el proceso
de testing y auditoría del sistema.  
Se presenta como un **modelo de trabajo aplicado**, independientemente del grado
de avance del análisis, y no implica cobertura exhaustiva de todas las
funcionalidades del sistema.

### 1. Reconocimiento del sistema
Exploración inicial del sistema a partir de la navegación directa, sin
suposiciones previas ni documentación funcional formal.
Identificación de módulos visibles, acciones disponibles y flujos aparentes.

### 2. Identificación del flujo feliz mínimo
Ejecución del recorrido básico esperado por el sistema para una acción principal
(alta, carga o búsqueda), utilizando datos controlados o ficticios.
Observación de validaciones, mensajes y estados resultantes.

### 3. Exploración de flujos alternativos
Pruebas fuera del recorrido esperado: cargas incompletas, datos no normalizados,
repetición de acciones y navegación no lineal.
Detección de estados ambiguos o comportamientos no comunicados al usuario.

### 4. Observación transversal de usabilidad y accesibilidad
Análisis de feedback visual, mensajes de error, persistencia de estado y
comprensión de la interfaz.
Identificación de barreras de uso y accesibilidad desde una perspectiva de
usuario no experto y uso real del sistema.

### 5. Registro y tipificación de hallazgos
Documentación de los problemas observados de forma abstracta y anoniminizada,
priorizando patrones, impacto operativo y riesgos potenciales por sobre
incidencias aisladas.

### 6. Delimitación del alcance
Definición explícita de los aspectos analizados y de aquellos que quedaron fuera
del alcance del presente caso de estudio.


## Hallazgos generales (resumen)
- Falta de mensajes de confirmación en acciones críticas.
- Validaciones insuficientes para cargas con datos reales.
- Persistencia de estados o búsquedas sin indicación clara.
- Barreras de accesibilidad en formularios y feedback visual.

## Alcance
Este caso se centra en el análisis del comportamiento del sistema y su experiencia de uso.
No se exponen datos técnicos sensibles ni información institucional identificable.

## Nota sobre privacidad y confidencialidad
Este repositorio presenta un caso de estudio con fines profesionales y formativos.
Toda la información ha sido anonimizada.
No se incluyen datos reales, identificadores, URLs internas ni documentación confidencial.
