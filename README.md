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

## Pregunta: S061
**Planteamiento de la pregunta:**
¿Qué actividades debe llevar a cabo el responsable del tratamiento de datos en relación con el derecho de oposición?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_oposición(?do) ^ autogen0:derecho_cuenta_encargado(?do, ?dce) ^ autogen0:actividad_dentro_de_derecho_de_oposición(?dce, ?ado) -> sqwrl:select(?ado) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-61.png)

## Pregunta: S062
**Planteamiento de la pregunta:**
¿Cuántos días tiene el responsable del tratamiento de datos para atender las solicitudes de oposición?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_oposición(?do) ^ autogen0:derecho_cuenta_encargado(?do, ?dce) ^ autogen0:plazo_de_atención_en_días_para_el_derecho_de_oposición(?dce, ?pado) -> sqwrl:select(?pado) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-62.png)

## Pregunta: S063
**Planteamiento de la pregunta:**
¿Cuáles son las excepciones a los derechos de rectificación, actualización, eliminación y oposición?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Excepciones_de_derechos(?ed) ^ autogen0:derechos_para_rectificación_actualización_eliminación_y_oposición(?ed, ?edc) -> sqwrl:select(?edc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-63.png)

## Pregunta: S064
**Planteamiento de la pregunta:**
¿Cuáles son las condiciones para suspender el tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_a_la_suspensión_del_tratamiento(?dst) ^ autogen0:condiciones_para_la_suspensión_del_tratamiento(?dst, ?cst) -> sqwrl:select(?cst)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-64.png)

## Pregunta: S064
**Planteamiento de la pregunta:**
¿Cuáles son las condiciones para suspender el tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_a_la_suspensión_del_tratamiento(?dst) ^ autogen0:condiciones_para_la_suspensión_del_tratamiento(?dst, ?cst) -> sqwrl:select(?cst)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-64.png)

## Pregunta: S065
**Planteamiento de la pregunta:**
¿Dónde debe dirigirse el titular de los datos si experimenta problemas relacionados con la suspensión del tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Titular(?t) ^ autogen0:en_caso_de_suspesión_de_tratamiento_debe_recurrir_hacia(?t, ?st) -> sqwrl:select(?st)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-65.png)

## Pregunta: S066
**Planteamiento de la pregunta:**
¿Cuándo debe recurrir el titular de los datos a la autoridad de protección de datos personales respecto a la suspensión del tratamiento?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_a_la_suspensión_del_tratamiento(?dst) ^ autogen0:cuando_debe_ocurrir_el_titular_a_la_autoridad_de_protección_de_datos_personales(?dst, ?drapd) -> sqwrl:select(?drapd)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-66.png)

## Pregunta: S067
**Planteamiento de la pregunta:**
¿Cómo debe actuar el responsable del tratamiento ante la impugnación de la exactitud de los datos por parte del titular?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Titular(?t) ^ autogen0:en_caso_de_impugar_la_exactitud_de_los_datos_a(?t, ?tcidp) ^ autogen0:ante_impugnación_de_exactitud_de_datos(?tcidp, ?idp) -> sqwrl:select(?idp)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-67.png)

## Pregunta: S068
**Planteamiento de la pregunta:**
¿Bajo qué circunstancias pueden tratarse los datos personales impugnados en el derecho a la suspensión?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_a_la_suspensión_del_tratamiento(?dst) ^ autogen0:supuestos_para_tratar_los_datos_en_caso_de_impugnación_de_los_mismos(?dst, ?stdcidp) -> sqwrl:select(?stdcidp)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-68.png)

## Pregunta: S069
**Planteamiento de la pregunta:**
¿Qué actividades puede realizar el titular de los datos en caso de valoraciones automatizadas?

**Consulta en lenguaje SQWRL:**  
```
autogen0:en_caso_de_valoraciones_automatizadas(?t, ?cda) ^ autogen0:Derecho_a_no_ser_objeto_de_valoraciones_automatizadas(?dnva) ^ autogen0:para_el(?dnva, ?t) -> sqwrl:select(?cda)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-69.png)

## Pregunta: S070
**Planteamiento de la pregunta:**
¿En qué escenarios no se aplica el derecho a no ser objeto de decisiones basadas en valoraciones automatizadas?

**Consulta en lenguaje SQWRL:**  
```
autogen0:derechos_para_no_ser_objeto_de_valoraciones_automatizadas(?ed, ?edva) ^ autogen0:Excepciones_de_derechos(?ed) -> sqwrl:select(?edva)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-70.png)

## Pregunta: S071
**Planteamiento de la pregunta:**
¿Es posible revocar el derecho a no ser sujeto de decisiones automatizadas a través de contratos previos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Excepciones_de_derechos(?ed) ^ autogen0:no_se_podrá_revocar_el_derecho_a_no_ser_objeto_de_valoraciones_automatizadas(?ed, ?rdova) -> sqwrl:select(?rdova)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-71.png)

## Pregunta: S072
**Planteamiento de la pregunta:**
¿Qué tipo de datos no pueden ser tratados bajo el derecho a no ser objeto de valoraciones automatizadas y en qué condiciones sí?

**Consulta en lenguaje SQWRL:**  
```
autogen0:no_se_podrán_tratar(?dova, ?ntd) ^ autogen0:Derecho_a_no_ser_objeto_de_valoraciones_automatizadas(?dova) ^ autogen0:datos_no_sujetos_a_tratamiento_según_el_derecho_a_no_ser_objeto_de_decisiones_automatizadas(?ntd, ?dnst) -> sqwrl:select(?dnst)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-72.png)

## Pregunta: S073
**Planteamiento de la pregunta:**
¿En qué circunstancias el tratamiento de datos puede estar sujeto a decisiones automatizadas conforme al derecho de no ser objeto de tales decisiones automatizadas?

**Consulta en lenguaje SQWRL:**  
```
autogen0:no_se_podrán_tratar(?dova, ?ntd) ^ autogen0:Derecho_a_no_ser_objeto_de_valoraciones_automatizadas(?dova) ^ autogen0:datos_sujetos_a_tratamiento_según_el_derecho_a_no_ser_objeto_de_decisiones_automatizadas(?ntd, ?dst) -> sqwrl:select(?dst)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-73.png)

## Pregunta: S074
**Planteamiento de la pregunta:**
¿A partir de qué edad puede dar el titular su consentimiento explícito para el tratamiento de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Titular(?t) ^ autogen0:puede_dar_consentimiento_explícito_para_el_tratamiento(?t, true) -> sqwrl:select(?t)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-74.png)

## Pregunta: S075
**Planteamiento de la pregunta:**
¿Qué características debe tener la consulta en el marco del derecho a la consulta?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_consulta(?dc) ^ autogen0:garatiza_que(?dc, ?gq) -> sqwrl:select(?gq)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-75.png)

## Pregunta: S076
**Planteamiento de la pregunta:**
¿En qué entidad se pueden consultar los datos personales según lo establecido en el derecho de consulta?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_consulta(?dc) ^ autogen0:dónde_puede_consultar(?dc, ?dpc) -> sqwrl:select(?dpc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-76.png)

## Pregunta: S077
**Planteamiento de la pregunta:**
¿Cuál es el concepto central asociado al ámbito del derecho de la educación digital en la LOPDP?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_a_la_educación_digital(?ded) ^ autogen0:derecho_al_acceso_y_disponibilidad(?ded, ?sdad) -> sqwrl:select(?sdad)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-77.png)

## Pregunta: S078
**Planteamiento de la pregunta:**
 ¿Quiénes son responsables de garantizar el derecho a la educación digital?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_a_la_educación_digital(?ded) ^ autogen0:garantizar_la_educación_digital(?ded, ?dged) -> sqwrl:select(?dged)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-78.png)

## Pregunta: S079
**Planteamiento de la pregunta:**
¿Sobre qué personas recae el carácter inclusivo de la educación digital?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_a_la_educación_digital(?ded) ^ autogen0:carácter_inclusivo_en(?ded, ?cied) -> sqwrl:select(?cied)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-79.png)

## Pregunta: S080
**Planteamiento de la pregunta:**
¿En qué consiste el ejercicio de derechos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Ejercicio_de_derechos(?ed) ^ autogen0:descripción(?ed, ?d) -> sqwrl:select(?d)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-80.png)

## Pregunta: S081
**Planteamiento de la pregunta:**
¿Quiénes deben proporcionar capacitación e información sobre el uso y tratamiento responsable de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Ejercicio_de_derechos(?ed) ^ autogen0:deben_dar_capacitación_y_proveer_información(?ed, ?ddc) -> sqwrl:select(?ddc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-81.png)

## Pregunta: S082
**Planteamiento de la pregunta:**
¿Cuáles son las categorías especiales de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Categorías_especiales_de_datos_personales(?cde) ^ autogen0:categorías_especiales_de_datos_personales_están_compuestos_por(?cde, ?ecp) -> sqwrl:select(?ecp) ^ sqwrl:limit(4)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-82.png)

## Pregunta: S083
**Planteamiento de la pregunta:**
¿Bajo qué circunstancias se puede realizar el procesamiento de datos sensibles, incluso cuando no es válido el tratamiento de datos sensibles?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_sensibles(?tds) ^ autogen0:escenarios_de_tratamiento_de_datos_sensibles(?tds, ?etds) -> sqwrl:select(?etds)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-83.png)

## Pregunta: S084
**Planteamiento de la pregunta:**
¿Quién tiene la autoridad para otorgar el consentimiento para el procesamiento de datos personales de una persona fallecida?

**Consulta en lenguaje SQWRL:**  
```
autogen0:cuenta_con_un(?tf, ?cu) ^ autogen0:Titular_fallecido(?tf) -> sqwrl:select(?cu)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-84.png)

## Pregunta: S085
**Planteamiento de la pregunta:**
¿Qué acciones pueden realizar los titulares de derechos sucesores en relación con el ejercicio de los derechos de una persona fallecida a la que representan?

**Consulta en lenguaje SQWRL:**  
```
autogen0:cuenta_con_un(?tf, ?cu) ^ autogen0:ejercicio_de_derechos_por_parte_del_titular_fallecido(?cu, ?ed) ^ autogen0:Titular_fallecido(?tf) -> sqwrl:select(?ed)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-85.png)

## Pregunta: S086
**Planteamiento de la pregunta:**
¿Qué aspectos permiten evaluar el tratamiento de datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_crediticios(?tdc) ^ autogen0:permitan_evaluar(?tdc, ?pe) -> sqwrl:select(?pe)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-86.png)

## Pregunta: S087
**Planteamiento de la pregunta:**
¿Qué información puede proporcionar el tratamiento de datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:para_informar_sobre(?tdc, ?pis) ^ autogen0:Tratamiento_de_datos_crediticios(?tdc) -> sqwrl:select(?pis)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-87.png)

## Pregunta: S088
**Planteamiento de la pregunta:**
¿Cuáles son las fuentes de las que pueden obtenerse los datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_crediticios(?tdc) ^ autogen0:fuentes_de_dónde_se_obtuvieron_los_datos_crediticios(?tdc, ?fdo) -> sqwrl:select(?fdo)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-88.png)

## Pregunta: S089
**Planteamiento de la pregunta:**
¿Con qué finalidad se puede llevar a cabo el tratamiento de datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_crediticios(?tdc) ^ autogen0:destinado(?tdc, ?tddc) -> sqwrl:select(?tddc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-89.png)

## Pregunta: S090
**Planteamiento de la pregunta:**
¿Qué acciones están restringidas en relación con el tratamiento de datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_crediticios(?tdc) ^ autogen0:no_se_podrá_hacer_con_el_tratamiento_de_datos_crediticios(?tdc, ?npad) -> sqwrl:select(?npad)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-90.png)

## Pregunta: S091
**Planteamiento de la pregunta:**
¿Cuáles son los derechos de los titulares de datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_los_titulares_de_datos_crediticios(?dtdc) ^ autogen0:derechos_de_los_titulares_de_datos_crediticios(?dtdc, ?dtd) -> sqwrl:select(?dtd)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-91.png)

## Pregunta: S092
**Planteamiento de la pregunta:**
¿Cuáles son las condiciones para garantizar el derecho de acceso para los titulares de datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_los_titulares_de_datos_crediticios(?dtdc) ^ autogen0:derecho_al_acceso_de_los_titulares_de_datos_crediticios(?dtdc, ?dadp) -> sqwrl:select(?dadp)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-92.png)

## Pregunta: S093
**Planteamiento de la pregunta:**
¿Cuáles son los mecanismos para asegurar el derecho de acceso a los datos personales de los titulares de datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_los_titulares_de_datos_crediticios(?dtdc) ^ autogen0:mecanismos_para_asegurar_el_derecho_de_acceso_del_titular_de_datos_crediticios(?dtdc, ?mada) -> sqwrl:select(?mada)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-93.png)

## Pregunta: S094
**Planteamiento de la pregunta:**
¿Qué acciones debe realizar el titular de datos crediticios con respecto al derecho de actualización, rectificación o eliminación de datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_los_titulares_de_datos_crediticios(?dtdc) ^ autogen0:derecho_de_actualización_rectificación_o_eliminación_del_titular_de_datos_crediticios(?dtdc, ?daredc) -> sqwrl:select(?daredc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-94.png)

## Pregunta: S095
**Planteamiento de la pregunta:**
¿Qué debe hacer la fuente de información respecto a la solicitud de actualización, rectificación o eliminación realizada por el titular de datos crediticios?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Derecho_de_los_titulares_de_datos_crediticios(?dtdc) ^ autogen0:fuente_de_información_actividad_frente_la_solicitud(?dtdc, ?afi) -> sqwrl:select(?afi)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-95.png)

## Pregunta: S096
**Planteamiento de la pregunta:**
¿Quiénes son responsables de tratar los datos personales relativos a la salud?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_relativos_a_salud(?tds) ^ autogen0:recolección_y_tratamiento_de_dato_relativo_a_salud(?tds, ?rtdrs) -> sqwrl:select(?rtdrs)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-96.png)

## Pregunta: S097
**Planteamiento de la pregunta:**
¿Es necesario el consentimiento del titular para el tratamiento de sus datos relativos a salud?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_relativos_a_salud(?tds) ^ autogen0:en_lo_que_respecta_a_el(?tds, ?ctds) ^ autogen0:para_datos_relativos_a_salud_sin_consentimiento(?ctds, ?cdrs) -> sqwrl:select(?cdrs)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-97.png)

## Pregunta: S098
**Planteamiento de la pregunta:**
¿En qué situaciones se puede realizar el tratamiento de datos sin la necesidad del consentimiento del titular?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_relativos_a_salud(?tds) ^ autogen0:escenarios_de_aplicación_para_el_tratamiento_de_datos_sin_consentimiento(?tds, ?eatds) -> sqwrl:select(?eatds)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-98.png)

## Pregunta: S099
**Planteamiento de la pregunta:**
¿Quién debe supervisar el tratamiento de datos cuando las actividades que involucran datos relativos a la salud están relacionadas con la gestión de los servicios de salud?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_relativos_a_salud(?tds) ^ autogen0:supervisar_el_tratamiento_en_actividades_de_gestión_de_servicio_de_salud(?tds, ?dst) -> sqwrl:select(?dst)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-99.png)

## Pregunta: S100
**Planteamiento de la pregunta:**
¿Quién es el responsable de otorgar la autorización para el tratamiento de datos relativos a la salud?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_relativos_a_salud(?tds) ^ autogen0:deberá_ser_autorizado_por(?tds, ?tdrsdsa) -> sqwrl:select(?tdrsdsa)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-100.png)

## Pregunta: S101
**Planteamiento de la pregunta:**
¿En qué circunstancias debe la autoridad de protección de datos personales autorizar el tratamiento de datos de salud?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_relativos_a_salud(?tds) ^ autogen0:deberá_ser_autorizado_por(?tds, ?tdrsdsa) ^ autogen0:acciones_respecto_al_tratamiento_de_datos_de_salud(?tdrsdsa, ?artds) -> sqwrl:select(?artds)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-101.png)

## Pregunta: S102
**Planteamiento de la pregunta:**
¿Qué requisitos deben cumplirse para obtener la autorización para el tratamiento de datos relativos a salud por parte de la Autoridad de Protección de Datos Personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:autorización_de_tratamiento_de_datos_de_salud_anonimizados(?tds, ?atds) ^ autogen0:Tratamiento_de_datos_relativos_a_salud(?tds) -> sqwrl:select(?atds)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-102.png)

## Pregunta: S103
**Planteamiento de la pregunta:**
¿Con qué fines pueden ser tratados los datos relativos a la salud dentro del Sistema Nacional de Salud por entidades públicas y privadas?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_relativos_a_salud(?tds) ^ autogen0:fines_del_tratamiento_de_datos_por_entes_privados_y_públicos(?tds, ?tdepp) -> sqwrl:select(?tdepp)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-103.png)

## Pregunta: S104
**Planteamiento de la pregunta:**
¿Bajo qué condiciones pueden los entes públicos y privados llevar a cabo el tratamiento de datos relacionados con la salud?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Tratamiento_de_datos_relativos_a_salud(?tds) ^ autogen0:escenarios_para_el_tratamiento_por_entes_privados_y_públicos(?tds, ?eptepp) -> sqwrl:select(?eptepp)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-104.png)

## Pregunta: S105
**Planteamiento de la pregunta:**
¿Cuáles son las obligaciones del responsable y encargado del tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Responsable_del_tratamiento(?rt) ^ autogen0:obligaciones(?rt, ?o) -> sqwrl:select(?o) ^ sqwrl:limit(16)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-105.png)

## Pregunta: S106
**Planteamiento de la pregunta:**
¿Cuándo se designará un delegado de protección de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Delegado_de_protección_de_datos_personales(?dpd) ^ autogen0:se_asignará_un_delegado_de_protección_de_datos(?dpd, ?adpd) -> sqwrl:select(?adpd)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-106.png)

## Pregunta: S107
**Planteamiento de la pregunta:**
¿Cuáles son las funciones del delegado de protección de datos en relación con las actividades de tratamiento de datos realizadas por el responsable y el encargado?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Delegado_de_protección_de_datos_personales(?dpd) ^ autogen0:funciones_del_rol(?dpd, ?fdd) -> sqwrl:select(?fdd) ^ sqwrl:limit(5)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-107.png)

## Pregunta: S108
**Planteamiento de la pregunta:**
¿Qué integrantes del sistema de protección de datos supervisarán las actividades asociadas al delegado de protección de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Delegado_de_protección_de_datos_personales(?dpd) ^ autogen0:deberá_ser_observado_por(?dpd, ?dop) -> sqwrl:select(?dop)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-108.png)

## Pregunta: S109
**Planteamiento de la pregunta:**
¿En qué circunstancias el responsable y el encargado del tratamiento deben realizar observaciones sobre el delegado de protección de datos?


**Consulta en lenguaje SQWRL:**  
```
autogen0:Delegado_de_protección_de_datos_personales(?dpd) ^ autogen0:deberá_ser_observado_por(?dpd, ?dop) ^ autogen0:observaciones_del_delegado(?dop, ?odd) -> sqwrl:select( ?odd) ^ sqwrl:limit(5)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-109.png)

## Pregunta: S110
**Planteamiento de la pregunta:**
¿Quién tiene la facultad de presentar reclamaciones sobre la forma en que se está llevando a cabo el tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Reclamaciones(?r) ^ autogen0:podrán_ser_hechas_por(?r, ?pshp) -> sqwrl:select(?pshp)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-110.png)

## Pregunta: S111
**Planteamiento de la pregunta:**
¿Hacia quién van dirigidas las reclamaciones?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Reclamaciones(?r) ^ autogen0:van_destinadas_hacia(?r, ?rvdh) -> sqwrl:select(?rvdh)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-111.png)

## Pregunta: S112
**Planteamiento de la pregunta:**
¿De qué maneras pueden realizarse las reclamaciones?


**Consulta en lenguaje SQWRL:**  
```
autogen0:Reclamaciones(?r) ^ autogen0:podrán_ser_hecha_de_forma(?r, ?psh) -> sqwrl:select(?psh)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-112.png)

## Pregunta: S113
**Planteamiento de la pregunta:**
¿A través de qué medios se pueden presentar las reclamaciones?

**Consulta en lenguaje SQWRL:**  
```
autogen0:podrán_ser_hecha_por_medios(?r, ?pshpm) ^ autogen0:Reclamaciones(?r) -> sqwrl:select(?pshpm)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-113.png)

## Pregunta: S114
**Planteamiento de la pregunta:**
¿Sobre qué asuntos pueden referirse las reclamaciones presentadas por el titular de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Reclamaciones(?r) ^ autogen0:reclamos_de(?r, ?rd) -> sqwrl:select(?rd)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-114.png)

## Pregunta: S115
**Planteamiento de la pregunta:**
¿Qué se puede presentar como parte de una reclamación?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Reclamaciones(?r) ^ autogen0:presentar_en_caso_de_reclamación(?r, ?pecr) -> sqwrl:select(?pecr)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-115.png)

## Pregunta: S116
**Planteamiento de la pregunta:**
¿Qué consideraciones deben tenerse al responder a una reclamación?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Reclamaciones(?r) ^ autogen0:contestar_la_reclamación(?r, ?cr) -> sqwrl:select(?cr)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-116.png)

## Pregunta: S117
**Planteamiento de la pregunta:**
¿Qué acciones deben tomarse antes de responder a una reclamación?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Reclamaciones(?r) ^ autogen0:antes_de_contestar_la_reclamación(?r, ?acr) -> sqwrl:select(?acr)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-117.png)

## Pregunta: S118
**Planteamiento de la pregunta:**
¿Qué acciones puede tomar el titular de los datos ante la negativa o falta de respuesta a una reclamación después de que haya vencido el plazo establecido de respuesta a la misma?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Reclamaciones(?r) ^ autogen0:ante_una_negación_o_no_respuesta_del_reclamo(?r, ?annr) -> sqwrl:select(?annr)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-118.png)

## Pregunta: S119
**Planteamiento de la pregunta:**
¿En qué situaciones se pueden aplicar medidas correctivas?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Medidas_correctivas(?mc) ^ autogen0:en_caso_de_incumplimiento_de(?mc, ?ecimc) -> sqwrl:select(?ecimc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-119.png)

## Pregunta: S120
**Planteamiento de la pregunta:**
¿Quién es responsable de imponer las medidas correctivas?

**Consulta en lenguaje SQWRL:**  
```
autogen0:serán_impuestas_por(?mc, ?mcsip) ^ autogen0:Medidas_correctivas(?mc) -> sqwrl:select(?mcsip) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-120.png)

## Pregunta: S121
**Planteamiento de la pregunta:**
¿Cuáles son las posibles medidas correctivas que pueden aplicarse?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Medidas_correctivas(?mc) ^ autogen0:cuáles_serán_las_medidas_correctivas(?mc, ?cmc) -> sqwrl:select(?cmc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-121.png)

## Pregunta: S122
**Planteamiento de la pregunta:**
¿Qué pautas deben seguirse antes de dictar medidas correctivas por parte de la autoridad de protección de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Medidas_correctivas(?mc) ^ autogen0:antes_de_dictar_las_medidas_correctivas(?mc, ?admc) -> sqwrl:select(?admc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-122.png)

## Pregunta: S123
**Planteamiento de la pregunta:**
¿En qué circunstancias se recurre a la utilización de medidas correctivas?


**Consulta en lenguaje SQWRL:**  
```
autogen0:Medidas_correctivas(?mc) ^ autogen0:casos_para_incurrir_en_medidas_correctivas(?mc, ?cimc) -> sqwrl:select(?cimc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-123.png)

## Pregunta: S124
**Planteamiento de la pregunta:**
¿Qué acciones tomará la autoridad de protección de datos personales frente a presuntas infracciones leves cometidas por el responsable o encargado del tratamiento de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Medidas_correctivas(?mc) ^ autogen0:por_infracciones_leves(?mc, ?mcil) -> sqwrl:select(?mcil)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-124.png)

## Pregunta: S125
**Planteamiento de la pregunta:**
¿Qué medidas adoptará la autoridad de protección de datos personales frente a presuntas infracciones graves cometidas por el responsable o encargado del tratamiento de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:por_infracciones_graves(?mc, ?mcig) ^ autogen0:Medidas_correctivas(?mc) -> sqwrl:select(?mcig)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-125.png)

## Pregunta: S126
**Planteamiento de la pregunta:**
¿Qué acciones llevará a cabo la autoridad de protección de datos personales frente a presuntas infracciones muy graves cometidas por el responsable o encargado del tratamiento de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:por_infracciones_muy_graves(?mc, ?mcimg) ^ autogen0:Medidas_correctivas(?mc) -> sqwrl:select(?mcimg)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-126.png)

## Pregunta: S127
**Planteamiento de la pregunta:**
¿Cuándo se considera una sanción leve por parte del responsable del tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:cometidas_por(?il, ?rt) ^ autogen0:Infracciones_leves(?il) ^ autogen0:Responsable_del_tratamiento(?rt) ^ autogen0:infracciones_leves(?rt, ?eil) -> sqwrl:select(?eil) ^ sqwrl:limit(5)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-127.png)

## Pregunta: S128
**Planteamiento de la pregunta:**
¿Cuándo se considera una sanción grave por parte del responsable del tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Responsable_del_tratamiento(?rt) ^ autogen0:infracciones_graves(?rt, ?eig) ^ autogen0:Infracciones_graves(?ig) ^ autogen0:cometidas_por(?ig, ?rt) -> sqwrl:select(?eig) ^ sqwrl:limit(14)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-128.png)

## Pregunta: S129
**Planteamiento de la pregunta:**
¿Cuándo se considera una sanción leve por parte del encargado del tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Infracciones_leves(?il) ^ autogen0:cometidas_por(?il, ?et) ^ autogen0:infracciones_leves(?et, ?eil) ^ autogen0:Encargado_del_tratamiento(?et) -> sqwrl:select(?eil) ^ sqwrl:limit(4)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-129.png)

## Pregunta: S130
**Planteamiento de la pregunta:**
¿Cuándo se considera una sanción grave por parte del encargado del tratamiento de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:cometidas_por(?ig, ?et) ^ autogen0:Infracciones_graves(?ig) ^ autogen0:Encargado_del_tratamiento(?et) ^ autogen0:infracciones_graves(?et, ?eig) -> sqwrl:select(?eig) ^ sqwrl:limit(8)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-130.png)

## Pregunta: S131
**Planteamiento de la pregunta:**
¿Qué tipos de sanciones están incluidos en las sanciones?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones(?s) ^ autogen0:están_compuesto_por(?s, ?ec) -> sqwrl:select(?ec) ^ sqwrl:limit(2)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-131.png)

## Pregunta: S132
**Planteamiento de la pregunta:**
¿Quién será el encargado de imponer las sanciones en el sistema de protección de datos personales, independientemente de la gravedad de la sanción?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones(?s) ^ autogen0:serán_impuestas_por(?s, ?si) -> sqwrl:select(?si) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-132.png)

## Pregunta: S133
**Planteamiento de la pregunta:**
¿Hacia que tipo de personas pueden dirigirse las infracciones leves?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones_por_infracciones_leves(?sil) ^ destinadas(?sil, ?d) -> sqwrl:select(?d) ^ sqwrl:limit(2)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-133.png)

## Pregunta: S134
**Planteamiento de la pregunta:**
¿Cuáles son las multas y acciones por infracciones leves cuando están dirigidas hacia servidores o funcionarios públicos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones_por_infracciones_leves(?sil) ^ autogen0:tipo_de_sanción_por_infracciones_hacia_servidores_o_funcionarios_públicos(?sil, ?tssf) -> sqwrl:select(?tssf) ^ sqwrl:limit(2)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-134.png)

## Pregunta: S135
**Planteamiento de la pregunta:**
¿Cuáles son las multas y acciones por infracciones leves cuando están dirigidas hacia el responsable, el encargado del tratamiento o terceros?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones_por_infracciones_leves(?sil) ^ autogen0:tipo_de_sanción_por_infracciones_hacia_responsable_o_el_encargado_del_tratamiento(?sil, ?tsret) -> sqwrl:select(?tsret) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-135.png)

## Pregunta: S136
**Planteamiento de la pregunta:**
¿En base a qué se determina la multa cuando se cometen infracciones leves por parte del responsable, el encargado del tratamiento o terceros?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones_por_infracciones_leves(?sil) ^ autogen0:determinación_de_la_multa_respecto_a_sanciones_por_infracción_del_responsable_o_encargado_del_tratamiento(?sil, ?dm) -> sqwrl:select(?dm) ^ sqwrl:limit(4)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-136.png)

## Pregunta: S137
**Planteamiento de la pregunta:**
¿Hacia que tipo de personas pueden dirigirse las infracciones graves?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones_por_infracciones_graves(?sig) ^ destinadas(?sig, ?d) -> sqwrl:select(?d) ^ sqwrl:limit(2)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-137.png)

## Pregunta: S138
**Planteamiento de la pregunta:**
¿Hacia que tipo de personas pueden dirigirse las infracciones graves?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones_por_infracciones_graves(?sig) ^ autogen0:tipo_de_sanción_por_infracciones_hacia_servidores_o_funcionarios_públicos(?sig, ?tssf) -> sqwrl:select(?tssf) ^ sqwrl:limit(2)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-138.png)

## Pregunta: S139
**Planteamiento de la pregunta:**
¿Cuáles son las multas y acciones por infracciones graves cuando están dirigidas hacia el responsable, el encargado del tratamiento o terceros?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones_por_infracciones_graves(?sig) ^ autogen0:tipo_de_sanción_por_infracciones_hacia_responsable_o_el_encargado_del_tratamiento(?sig, ?tsret) -> sqwrl:select(?tsret) ^ sqwrl:limit(1)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-139.png)

## Pregunta: S140
**Planteamiento de la pregunta:**
¿En base a qué se determina la multa cuando se cometen infracciones graves por parte del responsable, el encargado del tratamiento o terceros?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Sanciones_por_infracciones_graves(?sig) ^ autogen0:determinación_de_la_multa_respecto_a_sanciones_por_infracción_del_responsable_o_encargado_del_tratamiento(?sig, ?dm) -> sqwrl:select(?dm) ^ sqwrl:limit(4)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-140.png)

## Pregunta: S141
**Planteamiento de la pregunta:**
¿Cuáles son las funciones y atribuciones asociadas con la autoridad de protección de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Autoridad_de_protección_de_datos_personales(?apd) ^ autogen0:funciones(?apd, ?f) -> sqwrl:select(?f)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-141.png)

## Pregunta: S142
**Planteamiento de la pregunta:**
¿Bajo qué otro nombre se conoce a la autoridad de protección de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Autoridad_de_protección_de_datos_personales(?apd) ^ autogen0:conocido_como(?apd, ?cm) -> sqwrl:select(?cm)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-142.png)

## Pregunta: S143
**Planteamiento de la pregunta:**
¿Cómo será designada la autoridad de protección de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Autoridad_de_protección_de_datos_personales(?apd) ^ autogen0:designación(?apd, ?d) -> sqwrl:select(?d)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-143.png)

## Pregunta: S144
**Planteamiento de la pregunta:**
¿Cuáles son los requisitos que debe cumplir la autoridad de protección de datos para ser designada como autoridad de datos personales?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Autoridad_de_protección_de_datos_personales(?apd) ^ autogen0:requisitos_que_debe_cumplir(?apd, ?rdc) -> sqwrl:select(?rdc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-144.png)

## Pregunta: S145
**Planteamiento de la pregunta:**
¿Cuál será la duración del cargo de la autoridad de protección de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Autoridad_de_protección_de_datos_personales(?apd) ^ autogen0:duración_del_cargo(?apd, ?dc) -> sqwrl:select(?dc)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-145.png)

## Pregunta: S146
**Planteamiento de la pregunta:**
¿Cuáles son las razones para revocar el mandato de la autoridad de protección de datos?

**Consulta en lenguaje SQWRL:**  
```
autogen0:Autoridad_de_protección_de_datos_personales(?apd) ^ autogen0:revocación(?apd, ?r) -> sqwrl:select(?r)
```  
**Respuesta proporcionada por la ontología:**  
![alt text](image-146.png)




