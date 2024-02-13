# Preguntas relacionadas con la Ontología que cubre el ámbito del procesamiento y la recopilación de datos personales de acuerdo con lo establecido por la Ley Orgánica de Protección de Datos Personales.

A continuación, se presentan una serie de preguntas que la ontología puede responder en el ámbito de recolección y procesamiento de datos personales. Cada pregunta contendrá un identificador para facilitar su referencia, el planteamiento de la pregunta, la especificación en lenguaje SQWRL y las respuestas proporcionadas por la ontología.

## Pregunta: 
**Planteamiento de la pregunta:**

**Consulta en lenguaje SQWRL:**
```

```
**Respuesta proporcionada por la ontología**

## Pregunta: S001
**Planteamiento de la pregunta:**
¿Bajo qué conceptos la LOPDP no se puede aplicar?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Inaplicabilidad(?in) ^ autogen0:explicación_de_concepto_de_inaplicabilidad(?x, ?exp) ^ autogen0:es_la_no_aplicación_de_la_ley_en(?in, ?x) -> sqwrl:select(?x, ?exp)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](S001.png)  

## Pregunta: S002
**Planteamiento de la pregunta:**
¿Cuáles son los escenarios de aplicación territorial?

**Consulta en lenguaje SQWRL:**  
```
autogen0:se_aplica_la_ley_en(?t, ?apt) ^ autogen0:escenario_de_aplicación_territorial(?apt, ?esc) ^ autogen0:Territorial(?t) -> sqwrl:select(?apt, ?esc)
```
**Respuesta proporcionada por la ontología:**  
![alt text](image-2.png)  

## Pregunta: S003
**Planteamiento de la pregunta:**
¿Quiénes forman parte del sistema de protección de datos personales?


**Consulta en lenguaje SQWRL:**  
```
autogen0:Integrantes_del_sistema_de_protección_de_datos_personales(?int) ^ autogen0:están_compuesto_por(?int, ?p) -> sqwrl:select(?p) ^ sqwrl:limit(6)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-3.png)  

## Pregunta: S004
**Planteamiento de la pregunta:**
¿Cómo se clasifican los tipos de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tipos_de_datos(?td) ^ autogen0:tipos_de_datos_están_compuestos_por(?td, ?cp) ^ autogen0:descripción(?cp, ?d) -> sqwrl:select(?cp, ?d)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-4.png)  

## Pregunta: S005
**Planteamiento de la pregunta:**
¿Por quién es autorizada la entidad certificadora?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Entidad_certificadora(?ec) ^ autogen0:es_autorizada_por(?ec, ?x) -> sqwrl:select(?x)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-5.png)  

## Pregunta: S006
**Planteamiento de la pregunta:**
¿Qué característica tienen las fuentes de acceso público?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Fuente_accesible_al_público(?fp) ^ autogen0:tiene_la_característica_de_ser(?fp, ?tc) -> sqwrl:select(?tc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-6.png)  

## Pregunta: S007
**Planteamiento de la pregunta:**
¿Quién otorga los sellos de certificación?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sellos_de_protección_de_datos_personales(?sc) ^ autogen0:es_otorgada_por(?sc, ?x) -> sqwrl:select(?x)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-7.png)  

## Pregunta: S008
**Planteamiento de la pregunta:**
¿Qué aspectos afectan la vulnerabilidad de la seguridad de los datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Vulnerabilidad_de_la_seguridad_de_los_datos_personales(?vs) ^ autogen0:afecta_a(?vs, ?aa) -> sqwrl:select(?aa)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-8.png)  

## Pregunta: S009
**Planteamiento de la pregunta:**
¿Quién es el responsable de canalizar el ejercicio de derechos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:responsables_de_canalizar_el_ejercicio_de_derechos(?d, ?r) ^ autogen0:Derechos(?d) ^ autogen0:responsable_de_canalizar_el_ejercicio_de_derechos(?d, ?dr) -> sqwrl:select(?dr, ?r)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-9.png) 

## Pregunta: S010
**Planteamiento de la pregunta:**
¿Cuál es el significado de canalizar el ejercicio de derechos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derechos(?d) ^ autogen0:descripción_responsables_de_canalizar_el_ejercicio_de_derechos(?d, ?desc) -> sqwrl:select(?desc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-10.png)  

## Pregunta: S011
**Planteamiento de la pregunta:**
¿Existen limitaciones del ejercicio de derechos según las leyes complementarias?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derechos(?d) ^ autogen0:limitación_de_ejercicio_de_derechos_por_leyes_secundarias(?d, ?lm) -> sqwrl:select(?lm)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-11.png)  

## Pregunta: S012
**Planteamiento de la pregunta:**
¿Cuáles son las condiciones para el tratamiento legítimo de los datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos(?t) ^ autogen0:condiciones_para_el_tratamiento_legítmo(?t, ?tl) ^ autogen0:Consentimiento(?c) ^ autogen0:condiciones_para_el_tratamiento_legítmo(?c, ?tl) -> sqwrl:select(?tl)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-12.png)  








