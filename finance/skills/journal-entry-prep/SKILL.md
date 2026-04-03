---
name: journal-entry-prep
description: Prepare asientos contables con los debitos, creditos y documentacion de respaldo para el cierre de fin de mes, conforme a las normas contables argentinas (RT FACPCE y NIIF). Usado para registrar devengos, amortizaciones, depreciacion de bienes de uso, liquidacion de sueldos y cargas sociales, reconocimiento de ingresos y cualquier asiento contable manual.
user-invocable: false
---

# Preparacion de Asientos Contables - Normativa Argentina

**Importante**: Esta habilidad facilita los flujos de trabajo de asientos contables pero no proporciona asesoramiento profesional. Todos los asientos deben ser revisados por contadores publicos matriculados antes de su registracion. Marco normativo: Resoluciones Tecnicas FACPCE (RT 6, 9, 16, 17, 18, 26, 41), NIIF para entes que las aplican, y normativa impositiva AFIP vigente.

## Tipos de Asiento Estandar

### Devengos de Cuentas a Pagar
Registrar pasivos por bienes o servicios recibidos pero no facturados al cierre, conforme al principio de devengado (RT 17, seccion 4.1).

**Asiento tipico:**
- Debito: Cuenta de gastos (o activar si califica como bien de uso)
- - Credito: Deudas por servicios devengados / Provisiones
 
  - **Consideraciones clave:**
  - - Revertir en el periodo siguiente al recibir la factura real
    - - El credito fiscal IVA no es computable hasta recibir la factura del proveedor
      - - Para honorarios profesionales: verificar retencion de Ganancias e IIBB al momento del pago
        - - Consistencia en la metodologia de estimacion periodo a periodo
         
          - ### Depreciacion de Bienes de Uso e Intangibles
          - Registrar el cargo por depreciacion/amortizacion conforme a RT 17 (seccion 4.6) y RT 9.
         
          - **Asiento tipico:**
          - - Debito: Amortizacion de bienes de uso / Amortizacion de intangibles (por sector o centro de costos)
            - - Credito: Amortizacion acumulada de bienes de uso / Amortizacion acumulada de intangibles
             
              - **Metodos de depreciacion aceptados (RT 17):**
              - - Linea recta: (Costo - Valor residual) / Vida util estimada - el mas utilizado
                - - Unidades producidas: Basado en uso real vs total esperado
                  - - Suma de digitos: Metodo acelerado
                    - - Saldo decreciente: Cuando el patron de consumo de beneficios lo justifica
                     
                      - **Consideraciones clave:**
                      - - En contexto de alta inflacion (RT 6): los valores de origen deben expresarse en moneda homogenea; la depreciacion se calcula sobre valores reexpresados por IPC-INDEC
                        - - Distinguir entre amortizacion contable y amortizacion impositiva (Ley 20.628): generan diferencias temporarias sujetas a impuesto diferido (RT 18)
                          - - Verificar si aplica revaluacion tecnica de bienes de uso (RT 31 / opcion valor razonable NIIF)
                            - - Registrar bajas y desafectaciones (RT 17, seccion 4.6.3)
                             
                              - ### Amortizacion de Gastos Anticipados y Cargos Diferidos
                              - Imputar gastos anticipados al resultado segun su periodo de cobertura (RT 17, seccion 4.10).
                             
                              - **Asiento tipico:**
                              - - Debito: Cuenta de gasto (seguros, software, alquileres, etc.)
                                - - Credito: Gastos pagados por adelantado / Cargos diferidos
                                 
                                  - **Categorias comunes:**
                                  - - Primas de seguros (polizas anuales o plurianuales)
                                    - - Licencias de software y suscripciones
                                      - - Alquileres anticipados
                                        - - Contratos de mantenimiento prepagados
                                          - - Gastos preoperativos y de organizacion (amortizables hasta 5 anios - RT 9)
                                           
                                            - **Consideraciones clave:**
                                            - - Mantener cronograma con fecha inicio, fin y cuota mensual
                                              - - En contexto RT 6: reexpresar saldos por indice de precios (IPC o IPM segun corresponda)
                                                - - Verificar cancelaciones anticipadas que requieran amortizacion acelerada
                                                 
                                                  - ### Liquidacion de Sueldos y Cargas Sociales
                                                  - Registrar haberes y cargas sociales conforme a la LCT (Ley 20.744) y normativa AFIP vigente.
                                                 
                                                  - **Asientos tipicos:**
                                                 
                                                  - *Haberes brutos y descuentos al trabajador:*
                                                  - - Debito: Sueldos y jornales (por sector / centro de costos)
                                                    - - Credito: Remuneraciones a pagar
                                                      - - Debito: Remuneraciones a pagar (descuentos)
                                                        - - Credito: SIPA retenido empleado (11%)
                                                          - - Credito: PAMI retenido (3%)
                                                            - - Credito: Obra social retenida (3%)
                                                              - - Credito: Retencion Ganancias 4ta categoria (si corresponde - RG AFIP vigente)
                                                               
                                                                - *Cargas sociales a cargo del empleador:*
                                                                - - Debito: Cargas sociales (por sector)
                                                                  - - Credito: SIPA empleador (12% - verificar alicuota vigente segun actividad)
                                                                    - - Credito: PAMI empleador (2%)
                                                                      - - Credito: Obra social empleador (6%)
                                                                        - - Credito: ART (segun poliza - variable por actividad)
                                                                          - - Credito: Fondo Nacional de Empleo (1%)
                                                                           
                                                                            - *SAC (Sueldo Anual Complementario) - devengamiento mensual:*
                                                                            - - Debito: SAC devengado
                                                                              - - Credito: Provision SAC a pagar (1/12 del mejor salario del semestre)
                                                                               
                                                                                - *Provision de vacaciones:*
                                                                                - - Debito: Vacaciones devengadas
                                                                                  - - Credito: Provision vacaciones
                                                                                   
                                                                                    - **Consideraciones clave:**
                                                                                    - - Verificar alicuotas de contribuciones patronales segun actividad y regimen de reduccion vigente
                                                                                      - - El SAC se paga en junio y diciembre; devengar mensualmente
                                                                                        - - Presentar F.931 mensual en AFIP (declaracion jurada de cargas sociales)
                                                                                          - - Retenciones Ganancias 4ta: aplicar escala actualizada del RG AFIP vigente
                                                                                            - - Verificar cuota de discapacidad si corresponde (Ley 22.431)
                                                                                             
                                                                                              - ### Reconocimiento de Ingresos
                                                                                              - Reconocer ingresos conforme al principio de devengado (RT 17) o NIIF 15 segun el ente.
                                                                                             
                                                                                              - **Asientos tipicos:**
                                                                                             
                                                                                              - *Venta de bienes o servicios:*
                                                                                              - - Debito: Deudores por ventas / Clientes
                                                                                                - - Credito: Ventas / Ingresos por servicios
                                                                                                  - - Credito: IVA debito fiscal (alicuota general 21%, reducida 10,5% segun actividad - Ley 23.349)
                                                                                                   
                                                                                                    - *Anticipo recibido de cliente (ingreso diferido):*
                                                                                                    - - Debito: Caja / Banco
                                                                                                      - - Credito: Anticipos de clientes (pasivo)
                                                                                                       
                                                                                                        - *Reconocimiento del anticipo al entregar el bien/servicio:*
                                                                                                        - - Debito: Anticipos de clientes
                                                                                                          - - Credito: Ventas / Ingresos
                                                                                                           
                                                                                                            - **Criterios de reconocimiento - RT 17:**
                                                                                                            - - El proceso generador de ingresos esta practicamente terminado
                                                                                                              - - Se han transferido al comprador los riesgos y ventajas del bien
                                                                                                                - - El importe puede medirse de manera confiable
                                                                                                                  - - Para servicios: reconocer segun grado de avance (RT 17, seccion 4.5.2)
                                                                                                                   
                                                                                                                    - **Criterios - NIIF 15 (entes que aplican NIIF):**
                                                                                                                    - - Identificar el contrato y las obligaciones de desempeno separadas
                                                                                                                      - - Determinar el precio de la transaccion
                                                                                                                        - - Asignar el precio a cada obligacion de desempeno
                                                                                                                          - - Reconocer al satisfacer cada obligacion
                                                                                                                           
                                                                                                                            - **Tratamiento impositivo del IVA:**
                                                                                                                            - - Debito fiscal: al momento de facturacion o entrega (lo que ocurra primero)
                                                                                                                              - - Exportaciones: exentas de IVA con derecho a recupero del credito fiscal
                                                                                                                                - - Verificar si aplica percepcion de IVA (RG AFIP 2408 u otras RG vigentes)
                                                                                                                                 
                                                                                                                                  - ## Documentacion de Respaldo Requerida
                                                                                                                                 
                                                                                                                                  - Todo asiento debe incluir:
                                                                                                                                  - - **Descripcion**: Que registra y por que, con referencia al periodo
                                                                                                                                    - - **Calculo de respaldo**: Como se determinaron los importes (formula, planilla, fuente)
                                                                                                                                      - - **Documentos fuente**: Factura, remito, contrato, recibo, F.931, liquidacion de sueldos, etc.
                                                                                                                                        - - **Periodo contable**: Mes/anio al que corresponde el devengamiento
                                                                                                                                          - - **Preparador**: Quien lo preparo y cuando
                                                                                                                                            - - **Aprobacion**: Evidencia de revision conforme a la matriz de autorizacion
                                                                                                                                              - - **Indicador de reversion**: Si el asiento se revierte automaticamente y cuando
                                                                                                                                               
                                                                                                                                                - ## Matriz de Aprobacion
                                                                                                                                               
                                                                                                                                                - | Tipo de Asiento | Importe (ARS) | Aprobador |
                                                                                                                                                - |---|---|---|
                                                                                                                                                - | Recurrente estandar | Cualquier importe | Jefe de Contabilidad |
                                                                                                                                                - | No recurrente / manual | Hasta $500.000 | Jefe de Contabilidad |
                                                                                                                                                - | No recurrente / manual | $500.001 a $5.000.000 | Contador General / Controller |
                                                                                                                                                - | No recurrente / manual | Mas de $5.000.000 | Gerente Adm. y Finanzas / CFO |
                                                                                                                                                - | Consolidacion / apertura | Cualquier importe | Contador General o superior |
                                                                                                                                                - | Ajuste por inflacion (RT 6) | Cualquier importe | Contador General o superior |
                                                                                                                                                - | Ajuste de periodo anterior | Cualquier importe | Contador General o superior |
                                                                                                                                               
                                                                                                                                                - *Nota: Revisar umbrales periodicamente por el contexto inflacionario argentino.*
                                                                                                                                               
                                                                                                                                                - ## Lista de Verificacion Pre-Aprobacion
                                                                                                                                               
                                                                                                                                                - - [ ] Debitos igual a creditos (asiento equilibrado)
                                                                                                                                                  - [ ] - [ ] Periodo contable correcto (no registrar en periodo cerrado)
                                                                                                                                                  - [ ] - [ ] Codigos de cuenta correctos y apropiados
                                                                                                                                                  - [ ] - [ ] Importes matematicamente exactos con respaldo de calculo
                                                                                                                                                  - [ ] - [ ] Descripcion clara y suficiente para auditoria
                                                                                                                                                  - [ ] - [ ] Imputacion por sector / centro de costos correcta
                                                                                                                                                  - [ ] - [ ] Tratamiento coherente con periodos anteriores y politicas contables
                                                                                                                                                  - [ ] - [ ] Reversion automatica configurada correctamente para devengos
                                                                                                                                                  - [ ] - [ ] Documentacion de respaldo completa y referenciada
                                                                                                                                                  - [ ] - [ ] Importe dentro del nivel de autoridad del preparador
                                                                                                                                                  - [ ] - [ ] No es duplicado de asiento existente
                                                                                                                                                  - [ ] - [ ] Tratamiento impositivo correcto (IVA, Ganancias, IIBB)
                                                                                                                                                  - [ ] - [ ] En contexto RT 6: valores expresados en moneda homogenea (reexpresados por IPC-INDEC)
                                                                                                                                                 
                                                                                                                                                  - [ ] ## Errores Comunes a Detectar
                                                                                                                                                 
                                                                                                                                                  - [ ] - **Asientos desequilibrados**: Debitos no coinciden con creditos
                                                                                                                                                  - [ ] - **Periodo incorrecto**: Asiento en periodo cerrado o equivocado
                                                                                                                                                  - [ ] - **Signo incorrecto**: Debito ingresado como credito o viceversa
                                                                                                                                                  - [ ] - **Asientos duplicados**: Misma transaccion registrada dos veces
                                                                                                                                                  - [ ] - **Cuenta incorrecta**: Asiento en cuenta equivocada (especialmente codigos similares)
                                                                                                                                                  - [ ] - **Reversion faltante**: Devengamiento no configurado para reversion automatica
                                                                                                                                                  - [ ] - **Devengos desactualizados**: No actualizados por cambios en condiciones o importes
                                                                                                                                                  - [ ] - **Tipo de cambio incorrecto**: Asientos en moneda extranjera con TC erroneo (tipo BCRA o tipo pactado segun corresponda)
                                                                                                                                                  - [ ] - **IVA mal tratado**: Credito fiscal computado de facturas no recibidas, o debito fiscal no registrado en periodo correcto
                                                                                                                                                  - [ ] - **Error de corte (cut-off)**: Transaccion en periodo incorrecto segun fecha de entrega o prestacion
                                                                                                                                                  - [ ] - **Omision de ajuste por inflacion**: No reexpresar saldos en contexto RT 6 por IPC-INDEC
                                                                                                                                                  - [ ] - **Error de capitalizacion**: Gastos que deberian activarse o activos imputados a resultados incorrectamente
                                                                                                                                                  - [ ] - **Eliminacion intercompany faltante**: Asientos entre entidades sin eliminacion en la consolidacion
                                                                                                                                                  - [ ] 
