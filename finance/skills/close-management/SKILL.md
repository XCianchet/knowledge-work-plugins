---
name: close-management
description: Gestiona el proceso de cierre de mes con secuenciacion de tareas, dependencias y seguimiento del estado, incluyendo las obligaciones impositivas argentinas (vencimientos AFIP) y las tareas contables conforme a las RT FACPCE. Usado para planificar el calendario de cierre, hacer seguimiento del progreso e identificar obstaculos.
user-invocable: false
---

# Gestion del Cierre Mensual - Argentina

**Importante**: Esta habilidad facilita los flujos de trabajo de cierre pero no proporciona asesoramiento profesional. Todas las actividades deben ser revisadas por contadores publicos matriculados.

## Lista de Verificacion - Cierre de Fin de Mes

### Pre-cierre (ultimos 2-3 dias habiles del mes)
- [ ] Enviar recordatorios de fechas limite a todos los responsables de area
- [ ] - [ ] Confirmar procedimientos de cierre con Cuentas a Pagar, Cuentas a Cobrar, Liquidacion de Sueldos y Tesoreria
- [ ] - [ ] Verificar que todos los subsistemas esten operativos (ERP, liquidacion de sueldos, homebanking)
- [ ] - [ ] Realizar conciliacion bancaria preliminar (toda la actividad excepto el ultimo dia)
- [ ] - [ ] Revisar ordenes de compra abiertas para necesidades de devengamiento
- [ ] - [ ] Confirmar que el cronograma de liquidacion de sueldos se ajusta al plazo de cierre
- [ ] - [ ] Verificar el calendario de vencimientos AFIP del mes siguiente (IVA, Ganancias, IIBB, F.931, etc.)
- [ ] - [ ] Recopilar informacion sobre transacciones inusuales conocidas

- [ ] ### Dia 1 del Cierre (T+1: Primer dia habil tras el cierre)
- [ ] - [ ] Confirmar que todos los modulos del submayor completaron el procesamiento
- [ ] - [ ] Realizar devengos de cuentas a pagar (bienes/servicios recibidos sin factura)
- [ ] - [ ] Registrar asientos de liquidacion de sueldos y devengamiento de cargas sociales
- [ ] - [ ] Registrar ingresos y egresos de caja/banco hasta el cierre del mes
- [ ] - [ ] Registrar transacciones intercompany y confirmar con contrapartes
- [ ] - [ ] Conciliacion bancaria completa con extracto bancario final
- [ ] - [ ] Ejecutar amortizacion de bienes de uso desde el registro de activos
- [ ] - [ ] Amortizacion de gastos anticipados y cargos diferidos
- [ ] - [ ] Devengar SAC y vacaciones del periodo

- [ ] ### Dia 2 del Cierre (T+2)
- [ ] - [ ] Completar asientos de reconocimiento de ingresos y ajustes de anticipos de clientes
- [ ] - [ ] Registrar todos los devengos restantes
- [ ] - [ ] Conciliacion del submayor de creditos por ventas
- [ ] - [ ] Conciliacion del submayor de deudas comerciales
- [ ] - [ ] Registrar ajustes de inventario (si corresponde)
- [ ] - [ ] Revaluar saldos en moneda extranjera al TC del BCRA al cierre
- [ ] - [ ] Iniciar conciliaciones de cuentas del balance

- [ ] ### Dia 3 del Cierre (T+3)
- [ ] - [ ] Completar todas las conciliaciones de balance
- [ ] - [ ] Registrar asientos de ajuste identificados en conciliaciones
- [ ] - [ ] Completar conciliacion y eliminacion intercompany
- [ ] - [ ] Generar balance de sumas y saldos preliminar y estado de resultados
- [ ] - [ ] Realizar analisis preliminar de variaciones (flujos)
- [ ] - [ ] Investigar y resolver variaciones significativas

- [ ] ### Dia 4 del Cierre (T+4)
- [ ] - [ ] Registrar asiento de Impuesto a las Ganancias (corriente y diferido - RT 18)
- [ ] - [ ] Preparar asiento de ajuste por inflacion (RT 6) si corresponde: calcular RECPAM y reexpresar rubros no monetarios por IPC-INDEC
- [ ] - [ ] Verificar reserva legal y distribucion de resultados si corresponde
- [ ] - [ ] Finalizar todos los asientos contables - cierre blando (soft close)
- [ ] - [ ] Generar estados contables borrador (Resultado, Situacion Patrimonial, Flujo de Efectivo)
- [ ] - [ ] Realizar analisis de variaciones detallado y preparar explicaciones
- [ ] - [ ] Revision por parte de la gerencia de los estados contables e indicadores clave

- [ ] ### Dia 5 del Cierre (T+5)
- [ ] - [ ] Registrar ajustes finales de la revision de gerencia
- [ ] - [ ] Finalizar estados contables - cierre definitivo (hard close)
- [ ] - [ ] Bloquear el periodo en el ERP / sistema contable
- [ ] - [ ] Distribuir el paquete de informes financieros a los responsables
- [ ] - [ ] Actualizar presupuestos/proyecciones con los resultados reales
- [ ] - [ ] Verificar fechas de vencimiento de obligaciones impositivas del proximo periodo
- [ ] - [ ] Realizar retrospectiva del cierre - identificar mejoras de proceso

- [ ] ## Calendario de Obligaciones Impositivas Mensuales (Argentina)

- [ ] Las siguientes obligaciones tienen vencimientos mensuales fijos; verificar calendario AFIP vigente por CUIT:

- [ ] | Obligacion | Formulario | Periodicidad | Observacion |
- [ ] |---|---|---|---|
- [ ] | IVA | F.2002 / IVA web | Mensual | Vence segun terminacion CUIT, aprox. dia 18-22 |
- [ ] | Cargas sociales (SIPA, PAMI, OS) | F.931 | Mensual | Vence dias 7-17 segun CUIT |
- [ ] | Retenciones Ganancias (SICORE) | F.2118 / SICORE | Mensual | Vence segun quincena |
- [ ] | Retenciones IIBB (SIRCAR / prov.) | Segun provincia | Mensual | Vencimientos por provincia |
- [ ] | Impuesto a las Ganancias (anticipo) | F.713 | Mensual | 10 cuotas anuales |
- [ ] | Bienes Personales (anticipo) | F.770 | Mensual | Segun calendario AFIP |
- [ ] | Ingresos Brutos CM (Convenio Multilateral) | CM03 | Mensual | Vence dia 30 aprox. |
- [ ] | Ingresos Brutos (jurisdiccion local) | Segun jurisdiccion | Mensual o bimestral | |

- [ ] ## Secuenciacion de Tareas y Dependencias

- [ ] ### NIVEL 1 (Sin dependencias - pueden iniciarse en T+1):
- [ ] - Registracion de ingresos/egresos de caja y banco
- [ ] - Obtencion del extracto bancario
- [ ] - Liquidacion y asientos de sueldos
- [ ] - Amortizacion de bienes de uso
- [ ] - Amortizacion de gastos anticipados
- [ ] - Preparacion de devengos de cuentas a pagar
- [ ] - Registro de transacciones intercompany

- [ ] ### NIVEL 2 (Depende del Nivel 1):
- [ ] - Conciliacion bancaria (necesita: asientos de caja/banco + extracto)
- [ ] - Reconocimiento de ingresos (necesita: datos de facturacion/entrega finalizados)
- [ ] - Conciliacion del submayor de creditos por ventas (necesita: todos los asientos de ingresos/cobros)
- [ ] - Conciliacion del submayor de deudas comerciales (necesita: todos los asientos de compras/pagos)
- [ ] - Revaluacion de moneda extranjera (necesita: todos los asientos en ME registrados)
- [ ] - Devengos restantes (necesita: revision de toda la informacion fuente)

- [ ] ### NIVEL 3 (Depende del Nivel 2):
- [ ] - Todas las conciliaciones de balance (necesita: todos los asientos registrados)
- [ ] - Conciliacion intercompany (necesita: ambas entidades registradas)
- [ ] - Asientos de ajuste de conciliaciones
- [ ] - Balance de sumas y saldos preliminar

- [ ] ### NIVEL 4 (Depende del Nivel 3):
- [ ] - Impuesto a las Ganancias corriente y diferido (necesita: resultado antes de impuesto finalizado)
- [ ] - Ajuste por inflacion RT 6 (necesita: balance de sumas y saldos completo e indice IPC del mes)
- [ ] - Borrador de estados contables
- [ ] - Analisis de variaciones preliminar

- [ ] ### NIVEL 5 (Depende del Nivel 4):
- [ ] - Revision de gerencia
- [ ] - Ajustes finales
- [ ] - Cierre definitivo / bloqueo del periodo
- [ ] - Paquete de informes
- [ ] - Actualizacion de presupuestos

- [ ] ## Seguimiento del Estado del Cierre

- [ ] | Tarea | Responsable | Fecha limite | Estado | Bloqueante | Notas |
- [ ] |---|---|---|---|---|---|
- [ ] | [Nombre de tarea] | [Persona/rol] | [Dia T+N] | No iniciado / En proceso / Completo / Bloqueado | [Si bloqueado: causa] | [Notas] |

- [ ] **Definiciones de estado:**
- [ ] - **No iniciado**: La tarea aun no comenzo (puede estar esperando dependencias)
- [ ] - **En proceso**: La tarea se esta trabajando activamente
- [ ] - **Completo**: La tarea termino y fue revisada/aprobada
- [ ] - **Bloqueado**: No puede avanzar por dependencia, datos faltantes o problema
- [ ] - **En riesgo**: En proceso pero puede no cumplir su fecha limite

- [ ] ## Indicadores del Proceso de Cierre

- [ ] | Indicador | Definicion | Objetivo |
- [ ] |---|---|---|
- [ ] | Duracion del cierre | Dias habiles desde fin de mes hasta cierre definitivo | Reducir periodo a periodo |
- [ ] | Asientos post soft-close | Asientos registrados tras la revision de gerencia | Minimizar |
- [ ] | Tareas con retraso | Tareas completadas despues de su fecha limite | Cero |
- [ ] | Excepciones en conciliaciones | Partidas que requieren investigacion | Reducir |
- [ ] | Presentaciones AFIP fuera de termino | Declaraciones juradas presentadas con mora | Cero (evitar multas e intereses) |

- [ ] ## Cierre Acelerado (Objetivo 3 dias)

- [ ] ### Dia T+1:
- [ ] - Todos los asientos registrados (automatizados + manuales)
- [ ] - Todas las conciliaciones de submayores
- [ ] - Conciliacion bancaria
- [ ] - Conciliacion intercompany
- [ ] - Balance de sumas y saldos preliminar

- [ ] ### Dia T+2:
- [ ] - Todas las conciliaciones de balance
- [ ] - Impuesto a las Ganancias (corriente y diferido)
- [ ] - Ajuste por inflacion RT 6 (si corresponde)
- [ ] - Borrador de estados contables
- [ ] - Analisis de variaciones
- [ ] - Revision de gerencia

- [ ] ### Dia T+3:
- [ ] - Ajustes finales
- [ ] - Cierre definitivo
- [ ] - Paquete de informes
- [ ] - Actualizacion de presupuestos

- [ ] **Prerequisitos para cierre de 3 dias:**
- [ ] - Asientos recurrentes automatizados (amortizacion, devengos estandar)
- [ ] - Conciliacion continua durante el mes
- [ ] - Eliminacion intercompany automatizada
- [ ] - Actividades de pre-cierre completadas antes del fin de mes
- [ ] - Equipo empoderado con responsabilidades claras
- [ ] - Integracion en tiempo real entre subsistemas
- [ ] - Indice IPC-INDEC disponible rapidamente (generalmente primeros dias del mes siguiente)

- [ ] ## Mejora Continua del Proceso

- [ ] ### Problemas Comunes y Soluciones

- [ ] | Cuello de botella | Causa raiz | Solucion |
- [ ] |---|---|---|
- [ ] | Devengos tardios | Esperando confirmacion de gasto del area | Implementar estimacion continua; establecer fechas limite |
- [ ] | Asientos manuales lentos | Asientos recurrentes preparados manualmente | Automatizar en el ERP |
- [ ] | Conciliaciones lentas | Comenzar desde cero cada mes | Implementar conciliacion continua |
- [ ] | Retrasos intercompany | Esperando confirmacion de la contraparte | Automatizar conciliacion; establecer plazos mas estrictos |
- [ ] | Ajuste por inflacion demorado | Indice IPC no disponible a tiempo | Prever con estimacion preliminar; ajustar al publicarse el indice definitivo |
- [ ] | Cambios en revision de gerencia | Ajustes importantes descubiertos en revision | Mejorar proceso de revision preliminar |
- [ ] | Documentacion faltante | Buscar documentacion de ultimo momento | Mantener documentacion durante todo el mes |

- [ ] ### Preguntas de Retrospectiva del Cierre
- [ ] - ¿Que salio bien en este cierre que debemos continuar?
- [ ] - ¿Que tardo mas de lo previsto y por que?
- [ ] - ¿Que obstaculos encontramos y como podemos prevenirlos?
- [ ] - ¿Hubo sorpresas en los resultados financieros que debiamos haber detectado antes?
- [ ] - ¿Que podemos automatizar o simplificar para el proximo mes?
- [ ] - ¿Los vencimientos impositivos del proximo mes estan identificados y hay responsable asignado?
- [ ] 
