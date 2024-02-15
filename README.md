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
![alt text](./Imagenes_preguntas/S001.png)  

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

## Pregunta: S013
**Planteamiento de la pregunta:**
¿Qué se entiende por interés legítimo?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Interés_legítimo(?il) ^ autogen0:descripción(?il, ?ds) -> sqwrl:select(?ds)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-13.png)  

## Pregunta: S014
**Planteamiento de la pregunta:**
¿En qué situaciones se pueden tratar o comunicar los datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Consentimiento(?c) ^ autogen0:para_tratar_y_comunicar_datos_personales_se_debe(?c, ?ptc) -> sqwrl:select(?ptc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-14.png)

## Pregunta: S015
**Planteamiento de la pregunta:**
¿Cuáles son las condiciones para que el consentimiento sea válido?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Consentimiento(?c) ^ autogen0:válido(?c, ?cv) -> sqwrl:select(?cv)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-15.png)

## Pregunta: S016
**Planteamiento de la pregunta:**
¿Cuál es la descripción de vicios de consentimiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Vicios_de_consentimiento(?vc) ^ autogen0:descripción(?vc, ?ds) -> sqwrl:select(?ds) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-16.png)

## Pregunta: S017
**Planteamiento de la pregunta:**
¿Cuándo puede un titular revocar su consentimiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Consentimiento(?c) ^ autogen0:cuándo_puede_producirse(?c, ?cr) -> sqwrl:select(?cr)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-17.png)

## Pregunta: S018
**Planteamiento de la pregunta:**
¿Se necesita una justificación para la revocación del consentimiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Consentimiento(?c) ^ autogen0:justficación_del_revocamiento(?c, ?j) -> sqwrl:select(?j)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-18.png)

## Pregunta: S019
**Planteamiento de la pregunta:**
¿Qué deben garantizar los mecanismos de revocación del consentimiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:deben_ser(?mr, ?cds) ^ autogen0:Mecanismos_de_revocamiento(?mr) -> sqwrl:select(?cds)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-19.png)

## Pregunta: S020
**Planteamiento de la pregunta:**
¿Cómo deben ser los mecanismos de revocamiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Mecanismos_de_revocamiento(?mr) ^ autogen0:como_deben_ser(?mr, ?cds) -> sqwrl:select(?cds)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-20.png)

## Pregunta: S021
**Planteamiento de la pregunta:**
¿Quién establece los mecanismos de revocamiento del consentimiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:son_establecidos_por(?mr, ?e) ^ autogen0:Mecanismos_de_revocamiento(?mr) -> sqwrl:select(?e)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-21.png)

## Pregunta: S022
**Planteamiento de la pregunta:**
¿Cuál es el efecto legal de la revocación del consentimiento en relación con el tratamiento previamente realizado?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Revocamiento_del_consentimiento(?rc) ^ autogen0:antes_de_la_revocación_del_consentimiento_se_considera(?rt, ?tarc) ^ autogen0:respecto_al_tratamiento(?rc, ?rt) -> sqwrl:select(?tarc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-22.png)

## Pregunta: S023
**Planteamiento de la pregunta:**
¿Qué acciones se deben tomar al realizar el tratamiento bajo interés legítimo?

**Consulta en lenguaje SQWRL:**  
```
autogen0:bajo_interés_legítimo(?td, ?tbil) ^ autogen0:Tratamiento_de_datos(?td) -> sqwrl:select(?tbil)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-23.png)

## Pregunta: S024
**Planteamiento de la pregunta:**
¿Cuáles son las características que deben tener las finalidades asociadas al tratamiento de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Finalidad(?f) ^ autogen0:deberán_ser(?f, ?fds) -> sqwrl:select(?fds)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-24.png)

## Pregunta: S025
**Planteamiento de la pregunta:**
¿Se permite el tratamiento de datos si las finalidades para dicho tratamiento son distintas a las originalmente recogidas?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Finalidad(?f) ^ autogen0:es_distinta_a_la_recogida_de_datos_en_el(?f, ?df) ^ autogen0:para_finalidad_distinta(?df, ?tdf) -> sqwrl:select(?tdf)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-25.png)

## Pregunta: S026
**Planteamiento de la pregunta:**
¿Qué consideraciones se deben tener al tratar datos para finalidades distintas a las que fueron recogidas inicialmente?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Finalidad(?f) ^ autogen0:es_distinta_a_la_recogida_de_datos_en_el(?f, ?df) ^ autogen0:determinar_la_compatibilidad(?df, ?dct) -> sqwrl:select(?dct)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-26.png)

## Pregunta: S027
**Planteamiento de la pregunta:**
¿Qué criterios deben cumplir los datos personales para considerarlos bajo el principio de calidad?

**Consulta en lenguaje SQWRL:**  
```
autogen0:asociada_a(?c, ?td) ^ autogen0:para_cumplir_con_calidad_se_debe(?td, ?cc) ^ autogen0:Calidad(?c) -> sqwrl:select(?cc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-27.png)

## Pregunta: S028
**Planteamiento de la pregunta:**
¿Quién es responsable de validar el principio de calidad en el tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Calidad(?c) ^ autogen0:está_encargada_por_el(?c, ?ec) -> sqwrl:select(?ec)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-28.png)

## Pregunta: S029
**Planteamiento de la pregunta:**
¿Cuándo se considera que la inexactitud de los datos no es imputable?

**Consulta en lenguaje SQWRL:**  
```
autogen0:no_es_imputable_la_inexactitud_cuando(?dp, ?nii) ^ autogen0:Datos_personales(?dp) -> sqwrl:select(?nii)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-29.png)

## Pregunta: S030
**Planteamiento de la pregunta:**
¿Quién determina los plazos para la suspensión o revisión periódica de los datos personales en el proceso de conservación?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Conservación(?c) ^ autogen0:encargado_de_establecer_los_plazos_para_la_suspensión_o_revisión_periódica_dentro_del_tratamiento_de_datos_es(?c, ?cesr) -> sqwrl:select(?cesr)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-30.png)

## Pregunta: S031
**Planteamiento de la pregunta:**
¿En qué situaciones se puede llevar a cabo una conservación ampliada de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Conservación(?c) ^ autogen0:conservación_ampliada_de_tratamiento_de_datos_personales(?c, ?catdp) -> sqwrl:select(?catdp)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-31.png)

## Pregunta: S032
**Planteamiento de la pregunta:**
¿Qué tipos de medidas de seguridad pueden implementarse para proteger los datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Seguridad(?s) ^ autogen0:tipos_de_medidas_de_seguridad(?s, ?tdm) -> sqwrl:select(?tdm)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-32.png)

## Pregunta: S033
**Planteamiento de la pregunta:**
¿Quiénes son responsables de implementar las medidas de seguridad de los datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Seguridad(?s) ^ autogen0:encargado_de_implementar_medidas_de_seguridad(?s, ?eims) -> sqwrl:select(?eims)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-33.png)

## Pregunta: S034
**Planteamiento de la pregunta:**
¿Qué actividades se deben realizar en relación con el principio de responsabilidad proactiva y demostrada por parte del responsable del tratamiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:actividad_respecto_a_responsabilidad_proactiva_y_demostrada(?r, ?arpd) ^ autogen0:Responsable_del_tratamiento(?r) -> sqwrl:select(?arpd)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-34.png)

## Pregunta: S035
**Planteamiento de la pregunta:**
¿Con qué debe cumplir el responsable del tratamiento de datos en relación con la responsabilidad proactiva?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Responsable_del_tratamiento(?r) ^ autogen0:debe_haber_cumplido_respecto_a_responsabilidad_proactiva(?r, ?dhacrrp) -> sqwrl:select(?dhacrrp)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-35.png)

## Pregunta: S036
**Planteamiento de la pregunta:**
¿Cuáles métodos pueden emplearse para asegurar que se están cumpliendo las actividades relacionadas con el principio de responsabilidad proactiva y demostrable?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Responsable_del_tratamiento(?r) ^ autogen0:acreditar_el_cumplimiento_de_los_mecanismos(?r, ?acm) -> sqwrl:select(?acm)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-36.png)

## Pregunta: S037
**Planteamiento de la pregunta:**
 ¿A quién debe rendir cuentas el responsable del tratamiento de datos en relación con el manejo de los datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:debe_rendir_cuentas_respecto_al_tratamiento_con(?r, ?rcc) ^ autogen0:Responsable_del_tratamiento(?r) -> sqwrl:select(?rcc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-37.png)

## Pregunta: S038
**Planteamiento de la pregunta:**
 ¿Quién tiene la responsabilidad de implementar el principio de independencia de control?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Independencia_de_control(?ic) ^ autogen0:es_supervisada_por(?ic, ?ics) -> sqwrl:select(?ics)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-38.png)

## Pregunta: S039
**Planteamiento de la pregunta:**
¿Cuáles son las acciones llevadas a cabo por la autoridad de protección de datos personales en relación con el principio de independencia de control?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Independencia_de_control(?ic) ^ autogen0:acciones_respecto_a_la_independencia_de_control(?ics, ?aric) ^ autogen0:es_supervisada_por(?ic, ?ics) -> sqwrl:select(?aric)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-39.png)

## Pregunta: S040
**Planteamiento de la pregunta:**
¿Qué tipos de datos están sujetos a regulaciones especializadas según normativas específicas?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Datos_en_materia_especializada(?dpme) ^ autogen0:tratamiento_regulado_en_normativa_especializada_en_materia_de(?dpme, ?trne) -> sqwrl:select(?trne)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-40.png)

## Pregunta: S041
**Planteamiento de la pregunta:**
¿Bajo qué principios están sujetos los datos en materia especializada?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Datos_en_materia_especializada(?dme) ^ autogen0:estarán_sujetos_a(?dme, ?es) -> sqwrl:select(?es)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-41.png)

## Pregunta: S042
**Planteamiento de la pregunta:**
¿Cuáles son los criterios mínimos que los datos en materia especializadas deben cumplir?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Datos_en_materia_especializada(?dme) ^ autogen0:deberán_cumplir_por_lo_mínimo_con(?dme, ?dcm) ^ autogen0:están_conformados_por(?dcm, ?cdc) ^ autogen0:descripción(?cdc, ?des) -> sqwrl:select(?cdc, ?des) ^ sqwrl:limit(3)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-42.png)

## Pregunta: S043
**Planteamiento de la pregunta:**
¿Qué debe ser comunicado en el derecho a la información?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_a_la_información(?di) ^ autogen0:cononcer_en_el_derecho_a_la_información(?di, ?ddc) -> sqwrl:select(?ddc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-43.png)

## Pregunta: S044
**Planteamiento de la pregunta:**
¿Qué debe ser comunicado en el derecho a la información?

**Consulta en lenguaje SQWRL:**  
```
autogen0:en_caso_de_obtención_de_datos_directo_por_el(?c, ?codt) ^ autogen0:Consentimiento(?c) ^ autogen0:obtención_de_datos_personales_directamente_por_el_titular(?codt, ?odpdt) -> sqwrl:select(?odpdt)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-44.png)

## Pregunta: S045
**Planteamiento de la pregunta:**
¿Qué procedimientos deben seguirse cuando los datos personales no se obtienen directamente del titular?

**Consulta en lenguaje SQWRL:**  
```
autogen0:en_caso_de_no_obteción_directa_por_el_titular(?t, ?cnodt) ^ autogen0:Consentimiento(?c) ^ autogen0:en_caso_de_no_obtención_de_datos_directo_por_el(?c, ?t) -> sqwrl:select(?cnodt)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-45.png)

## Pregunta: S046
**Planteamiento de la pregunta:**
¿Cuál es el método adecuado para transmitir información durante el proceso de consentimiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Consentimiento(?c) ^ autogen0:modo_en_que_se_podrá_transmitir_la_información_al_titular(?c, ?m) -> sqwrl:select(?m)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-46.png)

## Pregunta: S047
**Planteamiento de la pregunta:**
¿Qué características debe tener la información que se proporciona al titular de datos cuando los datos se obtienen directa o indirectamente de él?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Consentimiento(?c) ^ autogen0:caracteristicas_que_debe_tener_la_información_transferida_al_titular(?c, ?cdti) -> sqwrl:select(?cdti)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-47.png)

## Pregunta: S048
**Planteamiento de la pregunta:**
¿Quién es responsable de garantizar el cumplimiento del derecho de acceso?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_acceso(?da) ^ autogen0:derecho_cuenta_encargado(?da, ?dce) -> sqwrl:select(?dce) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-48.png)

## Pregunta: S049
**Planteamiento de la pregunta:**
¿Cuáles son las actividades que el responsable del tratamiento de datos debe llevar a cabo con respecto al derecho de acceso?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_acceso(?da) ^ autogen0:derecho_cuenta_encargado(?da, ?dce) ^ autogen0:actividad_dentro_de_derecho_de_acceso(?dce, ?ada) -> sqwrl:select(?ada) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-49.png)

## Pregunta: S050
**Planteamiento de la pregunta:**
¿Cuál es el plazo para atender las solicitudes de acceso por parte del responsable del tratamiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_acceso(?da) ^ autogen0:derecho_cuenta_encargado(?da, ?dce) ^ autogen0:plazo_de_atención_en_días_para_el_derecho_de_acceso(?dce, ?pad) -> sqwrl:select(?pad) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-50.png)

## Pregunta: S051
**Planteamiento de la pregunta:**
¿Quién es responsable de garantizar el derecho de rectificación y actualización?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_rectificación_y_actualización(?dra) ^ autogen0:derecho_cuenta_encargado(?dra, ?dce) -> sqwrl:select(?dce) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-51.png)

## Pregunta: S052
**Planteamiento de la pregunta:**
¿Qué actividades debe realizar el responsable del tratamiento de datos en relación con el derecho de rectificación y actualización?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_rectificación_y_actualización(?dra) ^ autogen0:derecho_cuenta_encargado(?dra, ?dce) ^ autogen0:actividad_dentro_de_derecho_de_rectificación_y_actualización(?dce, ?adra) -> sqwrl:select(?adra) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-52.png)

## Pregunta: S053
**Planteamiento de la pregunta:**
¿Cuál es el plazo para atender las solicitudes de rectificación y actualización?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_rectificación_y_actualización(?dra) ^ autogen0:derecho_cuenta_encargado(?dra, ?dce) ^ autogen0:plazo_de_atención_en_días_para_el_derecho_de_rectificación_y_actualización(?dce, ?p) -> sqwrl:select(?p) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-53.png)

## Pregunta: S054
**Planteamiento de la pregunta:**
¿Quién es el responsable de garantizar el derecho de eliminación?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_eliminación(?de) ^ autogen0:derecho_cuenta_encargado(?de, ?dce) -> sqwrl:select(?dce) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-54.png)

## Pregunta: S055
**Planteamiento de la pregunta:**
¿En qué circunstancias se pueden eliminar los datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_eliminación(?de) ^ autogen0:cuándo_se_puede_eliminar_los_datos_personales(?dce, ?cedp) -> sqwrl:select(?cedp) ^ sqwrl:limit(7)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-55.png)

## Pregunta: S056
**Planteamiento de la pregunta:**
¿Qué actividades lleva a cabo el responsable del tratamiento de datos dentro del derecho de eliminación?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_eliminación(?de) ^ autogen0:derecho_cuenta_encargado(?de, ?dce) ^ autogen0:actividad_dentro_de_derecho_de_eliminación(?dce, ?ade) -> sqwrl:select(?ade) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-56.png)

## Pregunta: S057
**Planteamiento de la pregunta:**
 ¿Cuál es el plazo de atención para las solicitudes de eliminación de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_eliminación(?de) ^ autogen0:derecho_cuenta_encargado(?de, ?dce) ^ autogen0:plazo_de_atención_en_días_para_el_derecho_de_eliminación(?dce, ?pde) -> sqwrl:select(?pde) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-57.png)

## Pregunta: S058
**Planteamiento de la pregunta:**
¿Quién es responsable de garantizar el derecho de oposición?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_oposición(?do) ^ autogen0:derecho_cuenta_encargado(?do, ?dce) -> sqwrl:select(?dce) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-58.png)

## Pregunta: S059
**Planteamiento de la pregunta:**
¿En qué situaciones puede oponerse el titular al tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:cuándo_se_puede_oponer_al_tratamiento(?do, ?cpot) ^ autogen0:Derecho_de_oposición(?do) -> sqwrl:select(?cpot)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-59.png)

## Pregunta: S060
**Planteamiento de la pregunta:**
¿Qué sucede con el tratamiento de datos en caso de mercadotecnia directa?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_oposición(?do) ^ autogen0:en_caso_de_mercadotécnia_directa(?do, ?md) -> sqwrl:select(?md)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-60.png)
























