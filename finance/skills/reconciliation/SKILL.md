---
name: reconciliation
description: Concilie cuentas comparando saldos del libro mayor con submayores, extractos bancarios, posicion fiscal ante AFIP o datos de terceros. Usado para conciliaciones bancarias, conciliacion de libros IVA con DDJJ, conciliacion de cargas sociales (F.931), conciliacion entre libro mayor y submayor, y conciliaciones intercompany.
argument-hint: <cuenta> [periodo]
---

# Conciliacion de Cuentas - Normativa Argentina

**Importante**: Esta habilidad facilita los flujos de trabajo de conciliacion pero no proporciona asesoramiento profesional. Todas las conciliaciones deben ser revisadas por contadores publicos matriculados antes de su aprobacion.

## Tipos de Conciliacion

### 1. Conciliacion Bancaria
Comparar el saldo de la cuenta banco en el libro mayor con el saldo del extracto bancario.

**Proceso:**
1. Obtener el extracto bancario al cierre del periodo
2. 2. Obtener el saldo de la cuenta Banco en el libro mayor a la misma fecha
   3. 3. Identificar cheques emitidos pendientes de cobro (acreditados en libros, no debitados en banco)
      4. 4. Identificar depositos en transito (acreditados en libros, no acreditados en banco)
         5. 5. Identificar cargos bancarios, intereses, comisiones y retenciones no registradas en libros
            6. 6. Identificar acreditaciones bancarias automaticas no registradas (transferencias recibidas, intereses, etc.)
               7. 7. Conciliar ambos lados hasta obtener saldo ajustado coincidente
                 
                  8. **Formato estandar:**
                 
                  9. ```
                     CONCILIACION BANCARIA - [Nombre del banco] - [Periodo]

                     Saldo segun extracto bancario:           $XX.XXX
                     Mas: Depositos en transito               $X.XXX
                     Menos: Cheques pendientes de cobro      ($X.XXX)
                     Mas/Menos: Errores del banco             $X.XXX
                     Saldo bancario ajustado:                 $XX.XXX

                     Saldo segun libros contables:            $XX.XXX
                     Mas: Acreditaciones no registradas       $X.XXX
                     Menos: Debitos no registrados           ($X.XXX)
                       Comisiones bancarias                  ($X.XXX)
                       Impuesto al cheque (ITF - 0,6%)       ($X.XXX)
                       Retenciones aplicadas por el banco    ($X.XXX)
                     Mas/Menos: Errores en libros             $X.XXX
                     Saldo en libros ajustado:               $XX.XXX

                     Diferencia:                              $0,00
                     ```

                     **Consideraciones especificas Argentina:**
                     - Impuesto a las Transacciones Financieras (ITF, Ley 25.413): el banco debita automaticamente el 0,6% sobre debitos y creditos. Verificar que este registrado en libros como gasto o como pago a cuenta de Ganancias (si el ente es responsable inscripto)
                     - - Retenciones de Ganancias e IIBB practicadas por clientes al acreditar pagos: identificar en extracto y registrar contra la cuenta de retenciones a recuperar
                       - - Percepciones cobradas por el banco: verificar tratamiento (pago a cuenta o gasto)
                         - - Acreditaciones por transferencias: identificar origen y registrar correctamente
                           - - En cuentas en dolares: aplicar TC del BCRA al cierre para comparar con saldo contable reexpresado
                            
                             - ### 2. Conciliacion del Libro Mayor con el Submayor
                             - Comparar el saldo de la cuenta de control del libro mayor con el saldo del submayor detallado.
                            
                             - **Cuentas mas comunes a conciliar:**
                             - - Creditos por ventas (libro mayor vs submayor de deudores / analisis de antiguedad)
                               - - Deudas comerciales (libro mayor vs submayor de proveedores)
                                 - - Bienes de uso (libro mayor vs registro de activos fijos)
                                   - - Bienes de cambio (libro mayor vs valorizacion de inventario)
                                     - - Gastos anticipados (libro mayor vs cronograma de amortizacion)
                                       - - Previsiones (libro mayor vs detalle de previsiones constituidas)
                                        
                                         - **Proceso:**
                                         - 1. Obtener saldo del libro mayor para la cuenta de control al cierre
                                           2. 2. Obtener el balance del submayor o informe detallado a la misma fecha
                                              3. 3. Comparar totales: deben coincidir si la contabilizacion es en tiempo real
                                                 4. 4. Investigar diferencias (momento de registracion, asientos manuales no reflejados, errores de interfaz)
                                                   
                                                    5. **Causas comunes de diferencias:**
                                                    6. - Asientos manuales registrados en la cuenta de control sin reflejo en el submayor
                                                       - - Transacciones del submayor aun no integradas al libro mayor
                                                         - - Diferencias de timing en registracion por lotes
                                                           - - Asientos de reclasificacion en el libro mayor sin ajuste del submayor
                                                             - - Errores de interfaz del sistema o registraciones fallidas
                                                              
                                                               - ### 3. Conciliacion de Libros IVA con Declaracion Jurada
                                                               - Verificar que los libros IVA (compras y ventas) coincidan con la DDJJ de IVA presentada ante AFIP.
                                                              
                                                               - **Proceso:**
                                                               - 1. Obtener el resumen del libro IVA ventas del periodo (debito fiscal bruto)
                                                                 2. 2. Obtener el resumen del libro IVA compras del periodo (credito fiscal computable)
                                                                    3. 3. Cotejar contra los importes declarados en el F.2002 / IVA web (AFIP)
                                                                       4. 4. Verificar que el saldo contable de la cuenta IVA (debito menos credito) coincida con la DDJJ
                                                                          5. 5. Identificar percepciones y retenciones de IVA registradas vs las acreditadas por AFIP (SICORE/SIAP)
                                                                            
                                                                             6. **Conciliacion de retenciones y percepciones:**
                                                                             7. - Retenciones sufridas: cotejar constancias de retencion con lo declarado por los agentes de retencion en SICORE. Verificar que el monto a recuperar en libros coincida con el acumulado en la cuenta de AFIP
                                                                                - - Percepciones sufridas: verificar que las percepciones registradas coincidan con lo informado por los agentes
                                                                                 
                                                                                  - **Consideraciones clave:**
                                                                                  - - El IVA saldo tecnico (credito fiscal sin ventas gravadas suficientes) no genera acreditacion automatica; verificar si corresponde solicitar acreditacion, devolucion o transferencia (RG AFIP 1745 y ss.)
                                                                                    - - Para exportadores: verificar saldo acumulado de IVA recuperable y tramites de devolucion pendientes
                                                                                      - - Conciliar alicuotas aplicadas: 21%, 10,5%, exento, no gravado - verificar tratamiento correcto por tipo de operacion
                                                                                       
                                                                                        - ### 4. Conciliacion de Cargas Sociales (F.931)
                                                                                        - Verificar que las cargas sociales registradas contablemente coincidan con la DDJJ F.931 presentada en AFIP.
                                                                                       
                                                                                        - **Proceso:**
                                                                                        - 1. Obtener la liquidacion de haberes del periodo (total remuneraciones, contribuciones y aportes)
                                                                                          2. 2. Cotejar con la DDJJ F.931 presentada en AFIP
                                                                                             3. 3. Verificar que el saldo contable de las cuentas de cargas sociales a pagar coincida con lo declarado
                                                                                                4. 4. Verificar pagos realizados y saldo pendiente
                                                                                                   5. 5. Conciliar retenciones Ganancias 4ta categoria declaradas en SICORE vs registradas en libros
                                                                                                     
                                                                                                      6. **Consideraciones clave:**
                                                                                                      7. - Verificar que los aportes y contribuciones esten correctamente desagregados por concepto (SIPA, PAMI, OS, ART, FNE)
                                                                                                         - - Los pagos de cargas sociales tienen vencimientos especificos segun CUIT (verificar calendario de vencimientos AFIP)
                                                                                                           - - Las diferencias entre lo declarado y lo pagado generan deuda con AFIP (intereses resarcitorios y punitorios)
                                                                                                            
                                                                                                             - ### 5. Conciliacion Intercompany
                                                                                                             - Conciliar saldos entre entidades relacionadas para asegurar que se anulen en la consolidacion.
                                                                                                            
                                                                                                             - **Proceso:**
                                                                                                             - 1. Obtener saldos de cuentas por cobrar / pagar intercompany de cada entidad
                                                                                                               2. 2. Comparar el credito de la Entidad A con el debito de la Entidad B
                                                                                                                  3. 3. Identificar y resolver diferencias
                                                                                                                     4. 4. Confirmar que todas las transacciones intercompany esten registradas en ambas entidades
                                                                                                                        5. 5. Verificar que los asientos de eliminacion en la consolidacion sean correctos
                                                                                                                          
                                                                                                                           6. **Causas comunes de diferencias:**
                                                                                                                           7. - Transacciones registradas por una entidad pero no por la otra (timing)
                                                                                                                              - - Diferentes tipos de cambio utilizados por cada entidad (en operaciones en ME)
                                                                                                                                - - Clasificacion incorrecta (intercompany vs terceros)
                                                                                                                                  - - Importes disputados o pagos no aplicados
                                                                                                                                    - - Diferencias en la fecha de corte entre entidades
                                                                                                                                     
                                                                                                                                      - ## Categorizacion de Partidas de Conciliacion
                                                                                                                                     
                                                                                                                                      - **Categoria 1: Diferencias de Timing (se regularizaran solas)**
                                                                                                                                      - - Cheques emitidos pendientes de cobro
                                                                                                                                        - - Depositos en transito
                                                                                                                                          - - Transacciones contabilizadas en un sistema pendientes de interfaz al otro
                                                                                                                                            - - Aprobaciones pendientes
                                                                                                                                             
                                                                                                                                              - **Categoria 2: Requieren Asiento de Ajuste**
                                                                                                                                              - - Cargos bancarios no registrados (comisiones, ITF, gastos de mantenimiento)
                                                                                                                                                - - Intereses no registrados (ganados o perdidos)
                                                                                                                                                  - - Errores de registracion (importe incorrecto, cuenta incorrecta, duplicados)
                                                                                                                                                    - - Transacciones en un sistema sin asiento correspondiente en el otro
                                                                                                                                                      - - Errores de clasificacion (correcto importe, cuenta incorrecta)
                                                                                                                                                       
                                                                                                                                                        - **Categoria 3: Requieren Investigacion**
                                                                                                                                                        - - Diferencias no identificadas: variaciones sin causa obvia
                                                                                                                                                          - - Partidas en disputa: importes contestados entre las partes
                                                                                                                                                            - - Partidas vencidas: items que no se regularizaron en el plazo esperado
                                                                                                                                                              - - Diferencias recurrentes: mismo tipo de diferencia en cada periodo
                                                                                                                                                               
                                                                                                                                                                - ## Analisis de Antiguedad de Partidas Pendientes
                                                                                                                                                               
                                                                                                                                                                - | Antiguedad | Estado | Accion |
                                                                                                                                                                - |---|---|---|
                                                                                                                                                                - | 0-30 dias | Normal | Monitorear - dentro del ciclo normal |
                                                                                                                                                                - | 31-60 dias | En seguimiento | Investigar - seguimiento activo |
                                                                                                                                                                - | 61-90 dias | Vencida | Escalar al supervisor, documentar |
                                                                                                                                                                - | Mas de 90 dias | Critica | Escalar a gerencia - posible prevision o ajuste |
                                                                                                                                                               
                                                                                                                                                                - ## Umbrales de Escalada
                                                                                                                                                               
                                                                                                                                                                - | Disparador | Umbral (ejemplo) | Escalada |
                                                                                                                                                                - |---|---|---|
                                                                                                                                                                - | Importe de partida individual | Mayor a $100.000 | Revision del supervisor |
                                                                                                                                                                - | Importe de partida individual | Mayor a $500.000 | Revision del Contador General |
                                                                                                                                                                - | Total de partidas de conciliacion | Mayor a $1.000.000 | Revision del Contador General |
                                                                                                                                                                - | Antiguedad de la partida | Mas de 60 dias | Seguimiento supervisor |
                                                                                                                                                                - | Diferencia no resuelta con AFIP | Cualquier importe | Atencion inmediata - evitar intereses y multas |
                                                                                                                                                                - | Diferencia recurrente 3 periodos | Cualquier importe | Investigacion de proceso |
                                                                                                                                                               
                                                                                                                                                                - *Nota: Los umbrales deben revisarse periodicamente por el contexto inflacionario.*
                                                                                                                                                               
                                                                                                                                                                - ## Mejores Practicas
                                                                                                                                                               
                                                                                                                                                                - - **Oportunidad**: Realizar conciliaciones dentro del plazo del calendario de cierre (generalmente T+3 a T+5 habiles)
                                                                                                                                                                  - - **Integridad**: Conciliar todas las cuentas del balance a frecuencia definida (mensual para cuentas importantes, trimestral para las demas)
                                                                                                                                                                    - - **Documentacion**: Cada conciliacion debe incluir preparador, revisor, fecha y explicacion clara de todas las partidas
                                                                                                                                                                      - - **Segregacion**: Quien realiza la conciliacion no debe ser quien procesa las transacciones de esa cuenta
                                                                                                                                                                        - - **Seguimiento**: No dejar partidas pendientes indefinidamente; hacer seguimiento hasta su resolucion
                                                                                                                                                                          - - **Causa raiz**: Para partidas recurrentes, investigar y resolver el problema de proceso subyacente
                                                                                                                                                                            - - **Estandarizacion**: Usar plantillas y procedimientos consistentes en todas las cuentas
                                                                                                                                                                              - - **Retencion**: Conservar conciliaciones y documentacion de respaldo segun la politica de retencion de la organizacion y los plazos de prescripcion impositiva (generalmente 10 anios en Argentina)
                                                                                                                                                                                - 
