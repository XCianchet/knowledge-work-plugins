---
name: audit-support
description: Soporta el proceso de auditoria externa e interna conforme a las normas de auditoria argentinas (RT 37 FACPCE, NAA del CPCE, normas CNV para entes cotizantes). Incluye metodologia de pruebas de control, seleccion de muestras, estandares de documentacion y evaluacion de deficiencias. Reemplaza el enfoque SOX 404 por el marco de control interno argentino.
user-invocable: false
---

# Soporte de Auditoria - Normativa Argentina

**Importante**: Esta habilidad facilita los flujos de trabajo de auditoria pero no proporciona asesoramiento legal ni de auditoria. Todos los papeles de trabajo y evaluaciones deben ser revisados por contadores publicos matriculados e idoneamente habilitados. La "significatividad" y "materialidad" son conceptos que evaluan en ultima instancia los auditores.

Marco normativo: RT 37 FACPCE (Normas de Auditoria), Normas de Auditoria Aprobadas (NAA) de los CPCE provinciales, Normas de la CNV para entes que hacen oferta publica, e ISQC 1 / NIA para firmas que aplican normas internacionales.

## Marco de Control Interno en Argentina

A diferencia de la Ley Sarbanes-Oxley (SOX) de EE.UU., en Argentina no existe una norma equivalente de alcance universal obligatorio para el sector privado. Sin embargo, aplican los siguientes marcos segun el tipo de ente:

**Para entes que cotizan en CNV (oferta publica):**
- El auditor externo debe evaluar y reportar sobre el sistema de control interno en el informe de auditoria (RG CNV 622/2013 y ss.)
- - Se requiere Informe sobre el Sistema de Control Interno (ISCI) para ciertos entes
 
  - **Para entes en general:**
  - - La RT 37 FACPCE establece que el auditor debe comprender el control interno relevante para la auditoria
    - - El objetivo es evaluar el riesgo de error significativo y disenar procedimientos de auditoria apropiados
      - - No es obligatorio emitir opinion sobre la efectividad del control interno (salvo CNV u otros reguladores)
       
        - **Para el sector publico:**
        - - La Ley 24.156 (Administracion Financiera) establece el sistema de control interno (SIGEN) y externo (AGN)
         
          - ## Evaluacion del Riesgo de Auditoria
         
          - ### Componentes del Riesgo de Auditoria (RT 37)
          - - **Riesgo inherente**: Susceptibilidad de una afirmacion a un error significativo, sin considerar controles
            - - **Riesgo de control**: Probabilidad de que el sistema de control interno no prevenga o detecte el error
              - - **Riesgo de deteccion**: Probabilidad de que los procedimientos del auditor no detecten el error existente
               
                - ### Identificacion de Cuentas Significativas
               
                - Una cuenta es significativa si existe mas que una posibilidad remota de que pueda contener un error que sea material individualmente o en conjunto.
               
                - **Factores cuantitativos:**
                - - El saldo supera el umbral de materialidad (tipicamente 1-5% de un indicador de referencia: activo total, patrimonio neto, ingresos)
                  - - El volumen de transacciones es alto, incrementando el riesgo de error
                    - - La cuenta esta sujeta a estimaciones contables significativas
                     
                      - **Factores cualitativos:**
                      - - La cuenta involucra contabilidad compleja (reconocimiento de ingresos, ajuste por inflacion RT 6, VPP, deterioro de activos)
                        - - La cuenta es susceptible a fraude (efectivo, ingresos, transacciones con partes relacionadas)
                          - - Ha tenido errores o ajustes de auditoria en periodos anteriores
                            - - Involucra juicio significativo de la gerencia o estimaciones contables
                             
                              - ### Afirmaciones por Tipo de Cuenta
                             
                              - | Tipo de cuenta | Afirmaciones clave |
                              - |---|---|
                              - | Ingresos por ventas | Ocurrencia, Integridad, Exactitud, Corte |
                              - | Creditos por ventas | Existencia, Valuacion (prevision incobrables), Derechos |
                              - | Bienes de cambio | Existencia, Valuacion (costo vs. VNR), Integridad |
                              - | Bienes de uso | Existencia, Valuacion (costo o revaluo menos amort.), Integridad, Derechos |
                              - | Cuentas a pagar | Integridad, Exactitud, Existencia |
                              - | Cargas fiscales (IVA, IG, IIBB) | Integridad, Exactitud, Valuacion |
                              - | Pasivos laborales (SAC, vacaciones) | Integridad, Valuacion, Exactitud |
                              - | Patrimonio neto | Integridad, Exactitud, Presentacion |
                             
                              - ## Tipos de Procedimientos de Auditoria
                             
                              - ### Pruebas de Controles (cuando el auditor decide confiar en ellos)
                              - El auditor prueba si los controles operaron efectivamente durante el periodo bajo auditoria.
                             
                              - **Efectividad de diseno**: ¿El control esta correctamente disenado para prevenir o detectar un error significativo?
                              - - Evaluado mediante recorridos (walkthrough): trazar una transaccion de punta a punta
                                - - Confirmar que el control esta ubicado en el punto correcto del proceso
                                  - - Confirmar que el control aborda el riesgo identificado
                                   
                                    - **Efectividad operativa**: ¿El control opero segun lo disenado durante el periodo?
                                    - - Evaluado mediante pruebas (inspeccion, observacion, reejecucion, indagacion)
                                      - - Requiere tamanos de muestra suficientes para sustentar la conclusion
                                        - - Debe cubrir el periodo completo de confianza
                                         
                                          - ### Procedimientos Sustantivos
                                          - Los procedimientos sustantivos son obligatorios para cuentas significativas, independientemente de los controles.
                                         
                                          - **Tipos:**
                                          - - **Pruebas de detalle**: Confirmar saldos o transacciones individuales (confirmaciones, inspeccion de documentos, recalculo)
                                            - - **Procedimientos analiticos sustantivos**: Comparar saldos o ratios con expectativas del auditor
                                             
                                              - **Combinacion tipica:**
                                              - - Cuentas de bajo riesgo: principalmente procedimientos analiticos
                                                - - Cuentas de alto riesgo: mayormente pruebas de detalle, complementadas con analiticos
                                                 
                                                  - ## Seleccion de Muestras
                                                 
                                                  - ### Seleccion Aleatoria
                                                  - **Cuando usar**: Metodo por defecto para controles a nivel transaccion con poblaciones grandes.
                                                 
                                                  - **Metodo:**
                                                  - 1. Definir la poblacion (todas las transacciones sujetas al control durante el periodo)
                                                    2. 2. Numerar cada elemento secuencialmente
                                                       3. 3. Usar generador de numeros aleatorios para seleccionar items
                                                          4. 4. Asegurar que no hay sesgo en la seleccion
                                                            
                                                             5. **Ventajas**: Estadisticamente valido, defensible, sin sesgo de seleccion
                                                            
                                                             6. ### Seleccion Dirigida (Juicio del Auditor)
                                                             7. **Cuando usar**: Complemento a la seleccion aleatoria para pruebas basadas en riesgo; metodo principal cuando la poblacion es pequena o muy variable.
                                                            
                                                             8. **Metodo:**
                                                             9. - Seleccionar items con caracteristicas de riesgo especificas:
                                                                -   - Importe elevado (por encima de un umbral definido)
                                                                    -   - Transacciones inusuales o no estandar
                                                                        -   - Transacciones de fin de periodo (riesgo de corte)
                                                                            -   - Transacciones con partes relacionadas
                                                                                -   - Transacciones manuales o que implican anulaciones de controles
                                                                                    -   - Operaciones con proveedores o clientes nuevos
                                                                                     
                                                                                        - ### Guia de Tamano de Muestra
                                                                                     
                                                                                        - | Frecuencia del control | Poblacion | Muestra - Riesgo bajo | Muestra - Riesgo medio | Muestra - Riesgo alto |
                                                                                        - |---|---|---|---|---|
                                                                                        - | Anual | 1 | 1 | 1 | 1 |
                                                                                        - | Trimestral | 4 | 2 | 2 | 3 |
                                                                                        - | Mensual | 12 | 2 | 3 | 4 |
                                                                                        - | Semanal | 52 | 5 | 8 | 15 |
                                                                                        - | Diario | ~250 | 20 | 30 | 40 |
                                                                                        - | Por transaccion (pob. chica) | menos de 250 | 20 | 30 | 40 |
                                                                                        - | Por transaccion (pob. grande) | 250 o mas | 25 | 40 | 60 |
                                                                                     
                                                                                        - **Factores que incrementan el tamano de muestra:**
                                                                                        - - Mayor riesgo inherente en la cuenta/proceso
                                                                                          - - El control es el unico que atiende un riesgo significativo (sin controles compensatorios)
                                                                                            - - Deficiencia de control identificada en periodos anteriores
                                                                                              - - Control nuevo (no probado en periodos anteriores)
                                                                                                - - El auditor externo se apoya en el trabajo de auditoria interna
                                                                                                 
                                                                                                  - ## Estandares de Documentacion de Papeles de Trabajo
                                                                                                 
                                                                                                  - ### Requisitos del Papel de Trabajo (RT 37 FACPCE)
                                                                                                 
                                                                                                  - Todo papel de trabajo de prueba de control debe documentar:
                                                                                                 
                                                                                                  - **Identificacion del control:**
                                                                                                  - - Numero/ID del control
                                                                                                    - - Descripcion del control (que se hace, quien lo hace, con que frecuencia)
                                                                                                      - - Tipo de control (manual, automatizado, semi-automatizado)
                                                                                                        - - Frecuencia del control
                                                                                                          - - Riesgo y afirmacion que atiende
                                                                                                           
                                                                                                            - **Diseno de la prueba:**
                                                                                                            - - Objetivo de la prueba (que se quiere determinar)
                                                                                                              - - Procedimientos de prueba (instrucciones paso a paso)
                                                                                                                - - Evidencia esperada (que se espera ver si el control es efectivo)
                                                                                                                  - - Metodologia y razon de la seleccion de muestra
                                                                                                                   
                                                                                                                    - **Ejecucion de la prueba:**
                                                                                                                    - - Descripcion y tamano de la poblacion
                                                                                                                      - - Detalle de la seleccion de muestra (metodo, items seleccionados)
                                                                                                                        - - Resultado para cada item de la muestra (satisfactorio/excepcion, con evidencia especifica examinada)
                                                                                                                          - - Excepciones notadas con descripcion completa
                                                                                                                           
                                                                                                                            - **Conclusion:**
                                                                                                                            - - Evaluacion general (efectivo / deficiencia / deficiencia significativa / debilidad de control)
                                                                                                                              - - Base para la conclusion
                                                                                                                                - - Evaluacion del impacto de cualquier excepcion
                                                                                                                                  - - Controles compensatorios considerados (si aplica)
                                                                                                                                   
                                                                                                                                    - **Firma:**
                                                                                                                                    - - Nombre del preparador y fecha
                                                                                                                                      - - Nombre del revisor y fecha
                                                                                                                                       
                                                                                                                                        - ### Estandares de Evidencia Suficiente y Adecuada (RT 37)
                                                                                                                                       
                                                                                                                                        - **Evidencia suficiente y adecuada incluye:**
                                                                                                                                        - - Capturas de pantalla mostrando controles implementados en el sistema
                                                                                                                                          - - Documentos firmados/rubricados de aprobacion
                                                                                                                                            - - Aprobaciones por correo electronico con aprobador identificable y fecha
                                                                                                                                              - - Logs del sistema mostrando quien realizo la accion y cuando
                                                                                                                                                - - Calculos reejecucionados con resultados coincidentes
                                                                                                                                                  - - Notas de observacion (con fecha, lugar, observador)
                                                                                                                                                    - - Confirmaciones de terceros (bancos, clientes, proveedores)
                                                                                                                                                     
                                                                                                                                                      - **Evidencia insuficiente:**
                                                                                                                                                      - - Confirmaciones verbales solas (deben estar corroboradas)
                                                                                                                                                        - - Documentos sin fecha
                                                                                                                                                          - - Evidencia sin identificar al ejecutor/aprobador
                                                                                                                                                            - - Reportes genericos del sistema sin sello de fecha/hora
                                                                                                                                                              - - "Segun conversacion con [nombre]" sin documentacion de respaldo
                                                                                                                                                               
                                                                                                                                                                - ### Organizacion de los Papeles de Trabajo
                                                                                                                                                               
                                                                                                                                                                - ```
                                                                                                                                                                  Archivo de Auditoria - [Razon social] - Ejercicio [anio/mes cierre]
                                                                                                                                                                  ├── Legajo Permanente/
                                                                                                                                                                  │   ├── Informacion del ente (estatuto, actas, autorizaciones)
                                                                                                                                                                  │   ├── Contratos significativos
                                                                                                                                                                  │   ├── Politicas contables
                                                                                                                                                                  │   └── Estructura societaria
                                                                                                                                                                  ├── Legajo Corriente/
                                                                                                                                                                  │   ├── Planificacion y evaluacion de riesgo
                                                                                                                                                                  │   ├── Materialidad (determinacion y aplicacion)
                                                                                                                                                                  │   ├── Ingresos y cuentas a cobrar/
                                                                                                                                                                  │   │   ├── Programa de auditoria
                                                                                                                                                                  │   │   ├── Papeles de prueba (uno por procedimiento)
                                                                                                                                                                  │   │   └── Evidencia de respaldo
                                                                                                                                                                  │   ├── Compras y cuentas a pagar/
                                                                                                                                                                  │   ├── Nomina y cargas sociales/
                                                                                                                                                                  │   ├── Tesoreria/
                                                                                                                                                                  │   ├── Bienes de uso/
                                                                                                                                                                  │   ├── Impuestos (IVA, Ganancias, IIBB)/
                                                                                                                                                                  │   ├── Ajuste por inflacion (RT 6)/
                                                                                                                                                                  │   ├── Cierre contable y estados contables/
                                                                                                                                                                  │   └── Resumen y conclusiones/
                                                                                                                                                                  │       ├── Evaluacion de diferencias de auditoria
                                                                                                                                                                  │       ├── Diferencias ajustadas y no ajustadas
                                                                                                                                                                  │       └── Opinion del auditor (borrador)
                                                                                                                                                                  ```
                                                                                                                                                                  
                                                                                                                                                                  ## Clasificacion de Deficiencias de Control
                                                                                                                                                                  
                                                                                                                                                                  ### Deficiencia de Control
                                                                                                                                                                  Existe cuando el diseno u operacion de un control no permite a la gerencia o empleados, en el curso normal de sus funciones, prevenir o detectar errores oportunamente.
                                                                                                                                                                  
                                                                                                                                                                  **Factores de evaluacion:**
                                                                                                                                                                  - Probabilidad de que la falla del control resulte en un error significativo
                                                                                                                                                                  - - Magnitud del potencial error
                                                                                                                                                                    - - Existencia de controles compensatorios que mitiguen la deficiencia
                                                                                                                                                                     
                                                                                                                                                                      - ### Deficiencia Significativa
                                                                                                                                                                      - Una deficiencia, o combinacion de deficiencias, que merece atencion de quienes tienen a cargo el gobierno del ente (directorio, comision fiscalizadora, comite de auditoria).
                                                                                                                                                                     
                                                                                                                                                                      - **Indicadores:**
                                                                                                                                                                      - - Podria resultar en un error superior a insignificante pero inferior a material
                                                                                                                                                                        - - Mas que remota probabilidad de error material
                                                                                                                                                                          - - El control es clave y la deficiencia no esta totalmente mitigada por controles compensatorios
                                                                                                                                                                           
                                                                                                                                                                            - ### Debilidad de Control Material
                                                                                                                                                                            - Una deficiencia, o combinacion de deficiencias, tal que existe una posibilidad razonable de que un error material en los estados contables no sea prevenido o detectado oportunamente.
                                                                                                                                                                           
                                                                                                                                                                            - **Indicadores:**
                                                                                                                                                                            - - Identificacion de fraude por parte de la gerencia (cualquier magnitud)
                                                                                                                                                                              - - Reformulacion de estados contables de periodos anteriores para corregir un error material
                                                                                                                                                                                - - Identificacion por el auditor de un error material que los controles de la empresa no hubieran detectado
                                                                                                                                                                                  - - Supervision ineficaz por parte de la comision fiscalizadora o comite de auditoria
                                                                                                                                                                                    - - Deficiencia en un control persuasivo (nivel entidad, TI general) que afecta multiples procesos
                                                                                                                                                                                     
                                                                                                                                                                                      - ### Agregacion de Deficiencias
                                                                                                                                                                                      - Deficiencias individualmente no significativas pueden serlo en combinacion:
                                                                                                                                                                                      - - Identificar todas las deficiencias en el mismo proceso o que afectan la misma afirmacion
                                                                                                                                                                                        - - Evaluar si el efecto combinado podria resultar en un error material
                                                                                                                                                                                          - - Considerar si deficiencias en controles compensatorios agravan otras deficiencias
                                                                                                                                                                                            - - Documentar el analisis de agregacion y la conclusion
                                                                                                                                                                                             
                                                                                                                                                                                              - ### Remedicion
                                                                                                                                                                                              - Para cada deficiencia identificada:
                                                                                                                                                                                              - - **Analisis de causa raiz**: Por que fallo el control (falla de diseno, falla de ejecucion, personal, capacitacion, problema de sistema)
                                                                                                                                                                                                - - **Plan de accion**: Acciones especificas para corregir el control (rediseno, capacitacion adicional, mejora del sistema, revision adicional)
                                                                                                                                                                                                  - - **Fecha objetivo**: Cuando se completara la remedicion
                                                                                                                                                                                                    - - **Responsable**: Quien implementara la remedicion
                                                                                                                                                                                                      - - **Validacion**: Como y cuando se reprobara el control remediado para confirmar efectividad
                                                                                                                                                                                                       
                                                                                                                                                                                                        - ## Tipos de Controles
                                                                                                                                                                                                       
                                                                                                                                                                                                        - ### Controles de TI Generales (ITGC)
                                                                                                                                                                                                        - Controles sobre el ambiente de TI que apoyan el funcionamiento confiable de los controles de aplicacion.
                                                                                                                                                                                                       
                                                                                                                                                                                                        - - **Controles de acceso**: Provision de accesos (requieren aprobacion), baja de accesos de usuarios desvinculados, gestion de accesos privilegiados, revision periodica de accesos, politicas de contrasenas
                                                                                                                                                                                                          - - **Gestion de cambios**: Solicitudes documentadas y aprobadas antes de implementar, pruebas en ambiente no productivo, separacion entre desarrollo y produccion
                                                                                                                                                                                                            - - **Operaciones de TI**: Monitoreo de procesos batch, procedimientos de backup y recuperacion, disponibilidad del sistema, gestion de incidentes
                                                                                                                                                                                                             
                                                                                                                                                                                                              - ### Controles Manuales
                                                                                                                                                                                                              - Controles ejecutados por personas usando juicio.
                                                                                                                                                                                                             
                                                                                                                                                                                                              - **Ejemplos:**
                                                                                                                                                                                                              - - Revision gerencial de estados contables e indicadores clave
                                                                                                                                                                                                                - - Aprobacion supervisora de asientos contables por encima de un umbral
                                                                                                                                                                                                                  - - Verificacion de conciliaciones de cuentas
                                                                                                                                                                                                                    - - Aprobacion del libro de IVA y DDJJ antes de presentar a AFIP
                                                                                                                                                                                                                      - - Revision de la liquidacion de sueldos antes del pago
                                                                                                                                                                                                                        - - Aprobacion de pagos a proveedores (doble firma)
                                                                                                                                                                                                                         
                                                                                                                                                                                                                          - **Atributos clave a probar:**
                                                                                                                                                                                                                          - - El control fue ejecutado por la persona correcta (autoridad apropiada)
                                                                                                                                                                                                                            - - Se ejecuto oportunamente (dentro del plazo requerido)
                                                                                                                                                                                                                              - - Existe evidencia de la revision (firma, iniciales, correo electronico, log del sistema)
                                                                                                                                                                                                                                - - El revisor tuvo informacion suficiente para ejecutar una revision efectiva
                                                                                                                                                                                                                                  - - Las excepciones fueron identificadas y apropiadamente tratadas
                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                    - ### Controles Automatizados
                                                                                                                                                                                                                                    - Controles aplicados por sistemas de TI sin intervencion humana.
                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                    - **Ejemplos:**
                                                                                                                                                                                                                                    - - Flujos de aprobacion del sistema (no se puede continuar sin las aprobaciones requeridas)
                                                                                                                                                                                                                                      - - Deteccion de facturas duplicadas (el sistema bloquea o marca facturas duplicadas)
                                                                                                                                                                                                                                        - - Limite de credito (el sistema bloquea pedidos que superan el limite)
                                                                                                                                                                                                                                          - - Calculos automaticos (amortizacion, intereses, impuestos)
                                                                                                                                                                                                                                            - - Segregacion de funciones implementada por el sistema
                                                                                                                                                                                                                                             
                                                                                                                                                                                                                                              - **Enfoque de prueba:**
                                                                                                                                                                                                                                              - - Confirmar que la configuracion del sistema aplica el control segun lo disenado
                                                                                                                                                                                                                                                - - Para controles automatizados sin cambios, una sola prueba puede ser suficiente para el periodo (complementada con pruebas de ITGC de gestion de cambios)
                                                                                                                                                                                                                                                 
                                                                                                                                                                                                                                                  - ### Controles Manuales Dependientes de TI
                                                                                                                                                                                                                                                  - Controles manuales que se apoyan en la completitud y exactitud de informacion generada por el sistema.
                                                                                                                                                                                                                                                 
                                                                                                                                                                                                                                                  - **Ejemplos:**
                                                                                                                                                                                                                                                  - - Revision gerencial de un reporte de excepciones generado por el sistema
                                                                                                                                                                                                                                                    - - Supervision de un informe de antiguedad generado por el sistema para evaluar previsiones
                                                                                                                                                                                                                                                      - - Conciliacion usando el balance de sumas y saldos generado por el sistema
                                                                                                                                                                                                                                                        - - Aprobacion de transacciones identificadas por un flujo de trabajo del sistema
                                                                                                                                                                                                                                                         
                                                                                                                                                                                                                                                          - **Enfoque de prueba:**
                                                                                                                                                                                                                                                          - - Probar el control manual (revision, aprobacion, seguimiento de excepciones)
                                                                                                                                                                                                                                                            - - Y verificar la integridad y exactitud del reporte/datos subyacentes (IPE: Informacion Producida por el Ente)
                                                                                                                                                                                                                                                             
                                                                                                                                                                                                                                                              - ### Controles a Nivel Entidad
                                                                                                                                                                                                                                                              - Controles generales que operan a nivel organizativo y afectan multiples procesos.
                                                                                                                                                                                                                                                             
                                                                                                                                                                                                                                                              - **Ejemplos:**
                                                                                                                                                                                                                                                              - - Tono desde la cupula / codigo de conducta / politicas eticas
                                                                                                                                                                                                                                                                - - Proceso de evaluacion de riesgos
                                                                                                                                                                                                                                                                  - - Supervision del directorio / comision fiscalizadora / comite de auditoria
                                                                                                                                                                                                                                                                    - - Funcion y actividades de auditoria interna
                                                                                                                                                                                                                                                                      - - Evaluacion del riesgo de fraude
                                                                                                                                                                                                                                                                        - - Canal de denuncias (linea etica)
                                                                                                                                                                                                                                                                          - - Monitoreo de la efectividad del control por parte de la gerencia
                                                                                                                                                                                                                                                                            - - Proceso de presentacion de informes financieros al cierre (procedimientos de cierre, revisiones de cumplimiento RT)
                                                                                                                                                                                                                                                                             
                                                                                                                                                                                                                                                                              - **Significado:**
                                                                                                                                                                                                                                                                              - - Los controles a nivel entidad pueden mitigar, pero normalmente no pueden reemplazar, los controles a nivel proceso
                                                                                                                                                                                                                                                                                - - Controles ineficaces a nivel entidad (especialmente supervision del directorio y tono de la alta gerencia) son indicadores solidos de una debilidad material
                                                                                                                                                                                                                                                                                  - - Controles efectivos a nivel entidad pueden reducir la extension de las pruebas de controles a nivel proceso
                                                                                                                                                                                                                                                                                    - 
