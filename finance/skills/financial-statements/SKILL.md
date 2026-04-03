---
name: financial-statements
description: Genere estados contables (estado de resultados, estado de situacion patrimonial, estado de flujo de efectivo, estado de evolucion del patrimonio neto) con comparacion entre periodos y analisis de variaciones, conforme a las normas contables argentinas (RT FACPCE) o NIIF segun corresponda.
argument-hint: <frecuencia> <periodo>
---

# Estados Contables - Normativa Argentina

**Importante**: Esta habilidad facilita la preparacion de estados contables pero no proporciona asesoramiento profesional. Todos los estados contables deben ser revisados por contadores publicos matriculados antes de su uso. Marco normativo: RT 8, 9, 11, 16, 17, 26 FACPCE, y NIIF/NIC para entes que las adoptan.

Genera estados contables con comparacion entre periodos y analisis de variaciones. El flujo de trabajo cubre el estado de resultados; se incluyen formatos de referencia del estado de situacion patrimonial, estado de flujo de efectivo y estado de evolucion del patrimonio neto, conforme a la normativa argentina.

## Uso

`/financial-statements <tipo-periodo> <periodo>`

**Tipos de periodo:**
- `mensual` - Estado de resultados mensual con comparacion mes anterior y mismo mes anio anterior
- - `trimestral` - Estado de resultados trimestral con comparacion trimestre anterior y anio anterior
  - - `anual` - Estado contable anual completo con comparacion anio anterior
    - - `acumulado` - Estado acumulado del ejercicio con comparacion anio anterior
     
      - ## Flujo de Trabajo
     
      - ### 1. Recopilacion de Datos
     
      - Si el ERP o sistema contable esta conectado:
      - - Extraer datos del balance de sumas y saldos para el periodo
        - - Obtener datos del periodo de comparacion (periodo anterior, mismo periodo anio anterior, presupuesto)
          - - Extraer la estructura del plan de cuentas para la presentacion
           
            - Si no hay fuente de datos conectada:
            - - Solicitar al usuario el balance de sumas y saldos del periodo actual y de comparacion
              - - Solicitar ajustes y reclasificaciones conocidas
               
                - ### 2. Estado de Resultados (RT 8 / RT 9)
               
                - Presentar en formato multicolumna estandar:
               
                - ```
                  ESTADO DE RESULTADOS
                  Periodo: [descripcion del periodo]
                  (en miles de pesos, salvo indicacion contraria)

                                            Periodo    Periodo    Variacion  Variacion   Presup.   Var.
                                            Actual     Anterior      ($)        (%)       Anual    Pres.
                  INGRESOS POR VENTAS
                    Ventas de bienes        $XX.XXX    $XX.XXX    $X.XXX      X.X%      $XX.XXX   $X.XXX
                    Ingresos por servicios  $XX.XXX    $XX.XXX    $X.XXX      X.X%      $XX.XXX   $X.XXX
                    Otros ingresos          $XX.XXX    $XX.XXX    $X.XXX      X.X%      $XX.XXX   $X.XXX
                  TOTAL INGRESOS            $XX.XXX    $XX.XXX    $X.XXX      X.X%      $XX.XXX   $X.XXX

                  COSTO DE VENTAS           $XX.XXX    $XX.XXX    $X.XXX      X.X%      $XX.XXX   $X.XXX

                  RESULTADO BRUTO           $XX.XXX    $XX.XXX    $X.XXX      X.X%      $XX.XXX   $X.XXX
                    Margen bruto %          XX.X%      XX.X%

                  GASTOS DE ADMINISTRACION  $XX.XXX    $XX.XXX    $X.XXX      X.X%
                  GASTOS DE COMERCIALIZACION $XX.XXX   $XX.XXX    $X.XXX      X.X%
                  TOTAL GASTOS OPERATIVOS   $XX.XXX    $XX.XXX    $X.XXX      X.X%

                  RESULTADO OPERATIVO (EBIT) $XX.XXX   $XX.XXX    $X.XXX      X.X%
                    Margen operativo %      XX.X%      XX.X%

                  RESULTADOS FINANCIEROS Y POR TENENCIA
                    Intereses ganados       $XX.XXX    $XX.XXX    $X.XXX      X.X%
                    Intereses perdidos      ($XX.XXX)  ($XX.XXX)  $X.XXX      X.X%
                    Diferencia de cambio    $XX.XXX    $XX.XXX    $X.XXX      X.X%
                    Resultado por tenencia  $XX.XXX    $XX.XXX    $X.XXX      X.X%
                    RECPAM (Result. por exp.
                    al cambio en poder adq.) $XX.XXX   $XX.XXX    $X.XXX      X.X%
                  TOTAL RES. FINANCIEROS    $XX.XXX    $XX.XXX    $X.XXX      X.X%

                  RESULTADO ANTES DE IMPUESTO $XX.XXX  $XX.XXX    $X.XXX      X.X%

                  Impuesto a las Ganancias  ($XX.XXX)  ($XX.XXX)  $X.XXX      X.X%
                    Corriente               ($XX.XXX)
                    Diferido                ($XX.XXX)

                  RESULTADO DEL EJERCICIO   $XX.XXX    $XX.XXX    $X.XXX      X.X%      $XX.XXX   $X.XXX
                    Margen neto %           XX.X%      XX.X%
                  ```

                  ### 3. Analisis de Variaciones

                  Para cada linea, calcular y marcar variaciones significativas:

                  **Calculo de variaciones:**
                  - Variacion monetaria: Periodo actual - Periodo anterior (o actual - presupuesto)
                  - - Variacion porcentual: (Actual - Anterior) / |Anterior| x 100
                    - - Cambio en puntos basicos para margenes y ratios (1 pb = 0,01%)
                     
                      - **Umbrales de materialidad (ajustar por organizacion):**
                     
                      - | Tamano de la partida | Umbral monetario | Umbral porcentual |
                      - |---|---|---|
                      - | Mayor a $10M | $500K | 5% |
                      - | $1M a $10M | $100K | 10% |
                      - | Menor a $1M | $50K | 15% |
                     
                      - *Nota: En contexto inflacionario, comparar periodos en moneda homogenea (reexpresados por IPC-INDEC conforme RT 6)*
                     
                      - **Descomposicion de variaciones:**
                      - - Efecto volumen/cantidad: Cambio en volumen a precios del periodo anterior
                        - - Efecto precio/tarifa: Cambio en precio al volumen del periodo actual
                          - - Efecto mezcla: Cambio en la composicion del mix de productos/servicios
                            - - Partidas no recurrentes: Items que no se espera que se repitan
                              - - Efecto inflacion: Impacto del ajuste por IPC en la comparacion interperiodos
                                - - Efecto tipo de cambio: Impacto de variaciones del TC en operaciones en moneda extranjera
                                 
                                  - ### 4. Indicadores Clave
                                 
                                  - ```
                                    INDICADORES CLAVE           Actual    Anterior   Variacion
                                    Crecimiento de ventas (%)   X.X%
                                    Margen bruto (%)            XX.X%     XX.X%      X.X pp
                                    Margen operativo (%)        XX.X%     XX.X%      X.X pp
                                    Margen neto (%)             XX.X%     XX.X%      X.X pp
                                    Gastos adm. s/ventas (%)    XX.X%     XX.X%      X.X pp
                                    Gastos comerc. s/ventas (%) XX.X%     XX.X%      X.X pp
                                    Tasa efectiva IG (%)        XX.X%     XX.X%      X.X pp
                                    RECPAM s/resultado (%)      XX.X%     XX.X%      X.X pp
                                    ```

                                    ### 5. Resumen de Variaciones Significativas

                                    | Partida | Variacion ($) | Variacion (%) | Tipo | Causa preliminar | Accion |
                                    |---|---|---|---|---|---|
                                    | [Partida] | $X.XXX | X.X% | Desfav. | [si se conoce] | Investigar |

                                    ## Requisitos de Presentacion - Normativa Argentina

                                    ### Estado de Resultados (RT 8 / RT 9)

                                    - Clasificar gastos por funcion (administracion, comercializacion, produccion) — mas comun en Argentina — o por naturaleza
                                    - - Si se clasifican por funcion: revelar en notas la depreciacion, amortizacion y cargas sociales por naturaleza
                                      - - Presentar separadamente los resultados financieros y por tenencia
                                        - - Incluir el RECPAM (Resultado por Exposicion a Cambios en el Poder Adquisitivo de la Moneda) en contexto de ajuste por inflacion (RT 6)
                                          - - El Impuesto a las Ganancias se presenta como linea separada, discriminando corriente y diferido (RT 18)
                                            - - Las operaciones discontinuadas se presentan separadamente, netas de impuesto
                                              - - Para entes que aplican NIIF: clasificar otros resultados integrales (OCI) separadamente del resultado del periodo (NIC 1)
                                               
                                                - ### Estado de Situacion Patrimonial (RT 8 / RT 9)
                                               
                                                - - Clasificar activos y pasivos en corrientes y no corrientes (criterio: realizacion/vencimiento dentro de los 12 meses o del ciclo operativo si es mayor)
                                                  - - Presentar activos en orden decreciente de liquidez
                                                    - - Cuentas a cobrar: presentar netas de la prevision para deudores incobrables (RT 17, seccion 4.4)
                                                      - - Bienes de uso: presentar netos de amortizacion acumulada
                                                        - - En contexto RT 6: todos los rubros en moneda homogenea (fecha de cierre)
                                                          - - Inversiones en otras sociedades: metodo del valor patrimonial proporcional (RT 21) para significativas; costo o valor razonable para las demas
                                                           
                                                            - **Estructura del Estado de Situacion Patrimonial:**
                                                           
                                                            - ```
                                                              ACTIVO
                                                                ACTIVO CORRIENTE
                                                                  Caja y bancos
                                                                  Inversiones corrientes
                                                                  Creditos por ventas (neto de prevision)
                                                                  Otros creditos
                                                                  Bienes de cambio
                                                                  Activos por impuesto diferido corriente
                                                                  Otros activos corrientes
                                                                TOTAL ACTIVO CORRIENTE

                                                                ACTIVO NO CORRIENTE
                                                                  Creditos por ventas no corrientes
                                                                  Otros creditos no corrientes
                                                                  Inversiones permanentes (VPP)
                                                                  Bienes de uso (neto de amort. acumulada)
                                                                  Activos intangibles (neto de amort. acumulada)
                                                                  Llave de negocio
                                                                  Activos por impuesto diferido no corriente
                                                                  Otros activos no corrientes
                                                                TOTAL ACTIVO NO CORRIENTE

                                                              TOTAL ACTIVO

                                                              PASIVO
                                                                PASIVO CORRIENTE
                                                                  Deudas comerciales
                                                                  Deudas bancarias y financieras corrientes
                                                                  Remuneraciones y cargas sociales
                                                                  Cargas fiscales (IVA, Ganancias, IIBB, etc.)
                                                                  Anticipos de clientes
                                                                  Otros pasivos corrientes
                                                                TOTAL PASIVO CORRIENTE

                                                                PASIVO NO CORRIENTE
                                                                  Deudas bancarias y financieras no corrientes
                                                                  Previsiones (para contingencias, indemnizaciones)
                                                                  Pasivos por impuesto diferido
                                                                  Otros pasivos no corrientes
                                                                TOTAL PASIVO NO CORRIENTE

                                                              TOTAL PASIVO

                                                              PATRIMONIO NETO
                                                                  Capital social
                                                                  Ajuste del capital (RT 6)
                                                                  Aportes irrevocables a cuenta de futuras suscripciones
                                                                  Prima de emision
                                                                  Reserva legal
                                                                  Otras reservas
                                                                  Resultados no asignados
                                                                  Resultado del ejercicio
                                                              TOTAL PATRIMONIO NETO

                                                              TOTAL PASIVO Y PATRIMONIO NETO
                                                              ```

                                                              ### Estado de Flujo de Efectivo (RT 8 / RT 11)

                                                              - El metodo indirecto es el mas comun (partir del resultado del ejercicio, ajustar por partidas que no generan/usan efectivo)
                                                              - - El metodo directo esta permitido
                                                                - - Revelar intereses pagados e impuestos pagados (en el cuerpo o en notas)
                                                                  - - Las actividades no monetarias significativas se revelan en notas (por ejemplo, bienes incorporados por leasing, canjes)
                                                                    - - Efectivo y equivalentes: efectivo en caja y bancos mas inversiones de alta liquidez con vencimiento original hasta 3 meses
                                                                     
                                                                      - **Estructura del Estado de Flujo de Efectivo (Metodo Indirecto):**
                                                                     
                                                                      - ```
                                                                        FLUJOS DE EFECTIVO DE ACTIVIDADES OPERATIVAS
                                                                          Resultado del ejercicio
                                                                          Ajustes por partidas que no afectan el efectivo:
                                                                            Amortizacion de bienes de uso
                                                                            Amortizacion de intangibles
                                                                            RECPAM (si se aplica RT 6)
                                                                            Variacion de previsiones
                                                                            Resultado por venta de bienes de uso
                                                                            Impuesto a las Ganancias diferido
                                                                            Resultado del VPP en inversiones permanentes
                                                                          Cambios en activos y pasivos operativos:
                                                                            (Aumento) disminucion de creditos por ventas
                                                                            (Aumento) disminucion de bienes de cambio
                                                                            (Aumento) disminucion de otros creditos
                                                                            Aumento (disminucion) de deudas comerciales
                                                                            Aumento (disminucion) de cargas fiscales
                                                                            Aumento (disminucion) de remuneraciones y CS
                                                                            Aumento (disminucion) de anticipos de clientes
                                                                        FLUJO NETO DE ACTIVIDADES OPERATIVAS

                                                                        FLUJOS DE EFECTIVO DE ACTIVIDADES DE INVERSION
                                                                          Adquisicion de bienes de uso
                                                                          Cobros por venta de bienes de uso
                                                                          Adquisicion de activos intangibles
                                                                          Adquisicion de inversiones permanentes
                                                                          Cobros por venta de inversiones permanentes
                                                                          Cobros de dividendos
                                                                        FLUJO NETO DE ACTIVIDADES DE INVERSION

                                                                        FLUJOS DE EFECTIVO DE ACTIVIDADES DE FINANCIACION
                                                                          Obtencion de prestamos bancarios
                                                                          Cancelacion de prestamos bancarios
                                                                          Aportes de capital
                                                                          Pago de dividendos
                                                                          Recompra de acciones propias
                                                                        FLUJO NETO DE ACTIVIDADES DE FINANCIACION

                                                                        Efecto de las variaciones en el tipo de cambio sobre el efectivo
                                                                        VARIACION NETA EN EL EFECTIVO Y EQUIVALENTES
                                                                        Efectivo al inicio del periodo
                                                                        Efectivo al cierre del periodo
                                                                        ```

                                                                        ### Estado de Evolucion del Patrimonio Neto (RT 8)

                                                                        Presentar la variacion de cada rubro del PN durante el ejercicio:
                                                                        - Saldo al inicio del ejercicio
                                                                        - - Ajuste por inflacion (RT 6) si corresponde
                                                                          - - Dividendos distribuidos
                                                                            - - Absorcion de resultados no asignados
                                                                              - - Constituciones y desafectaciones de reservas
                                                                                - - Resultado del ejercicio
                                                                                  - - Otros resultados integrales (si aplica NIIF)
                                                                                    - - Saldo al cierre del ejercicio
                                                                                     
                                                                                      - ## Ajustes y Reclasificaciones de Cierre
                                                                                     
                                                                                      - **Ajustes tipicos:**
                                                                                      - - Devengos: registrar gastos incurridos no pagados (cargas sociales, intereses, honorarios)
                                                                                        - - Diferimientos: ajustar gastos anticipados y anticipos de clientes por el periodo
                                                                                          - - Depreciacion y amortizacion: correr desde el registro de bienes de uso
                                                                                            - - Prevision para deudores incobrables: ajustar segun analisis de antiguedad y experiencia historica
                                                                                              - - Ajuste de inventarios: registrar mermas, obsolescencia o bienes a valor de reposicion si es menor al costo
                                                                                                - - Revaluacion de moneda extranjera: convertir saldos en ME al TC del BCRA al cierre (RT 17, seccion 4.7)
                                                                                                  - - Impuesto a las Ganancias: registrar gasto corriente y diferido (RT 18)
                                                                                                    - - Ajuste por inflacion (RT 6): reexpresar todos los rubros no monetarios por indice IPC-INDEC si corresponde
                                                                                                     
                                                                                                      - **Reclasificaciones tipicas:**
                                                                                                      - - Corriente / no corriente: reclasificar deudas con vencimiento proximo a corriente
                                                                                                        - - Neteamiento de cuentas complementarias: amortizacion acumulada, prevision para incobrables
                                                                                                          - - Eliminacion de operaciones intercompany en consolidacion
                                                                                                            - - Operaciones discontinuadas: reclasificar como linea separada en el estado de resultados
                                                                                                              - - Metodo del VPP: actualizar inversiones en sociedades controladas/vinculadas (RT 21)
                                                                                                                - 
