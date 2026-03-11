# TelecomX - Análisis de Churn

## Propósito
Aplicar un proceso ETL y análisis de datos con Python para identificar los factores que influyen en la cancelación de clientes (churn) en TelecomX.

## Instrucciones de ejecución
1. Abrir `TelecomX_LATAM_2.ipynb` en Google Colab.
2. Cargar el archivo `telecomx_latam_limpio.csv`
3. Ejecutar las celdas en orden.
4. Dependencias: pandas, numpy, requests, matplotlib, seaborn, scikit-learn, imblearn.

## Resultados
- Churn general: ~27% de los clientes abandonan el servicio.
- Contrato mes a mes: ~42.7% de churn.
- Contratos de 1 o 2 años: menor tasa de cancelación.
- Cheque electrónico: mayor churn (~45%).
- Pagos automáticos: menor churn (~16%).
- Clientes con menor tiempo de permanencia tienen mayor probabilidad de cancelar.

## Limpieza y Tratamiento de Datos
- Importación del JSON desde GitHub.
- Normalización de estructuras anidadas.
- Estandarización de nombres de columnas.
- Conversión de variables a formato numérico.
- Manejo de valores faltantes.
- Codificación de variables binarias (yes/no → 1/0).
- Creación de la variable `cuentas_diarias`.

## Conclusión

### Factores más influyentes en churn
- Tipo de contrato
- Meses de permanencia (tenure)
- Cargos mensuales
- Método de pago
- Servicios adicionales (soporte técnico, seguridad)

### Análisis
- Contratos mes a mes presentan mayor churn.
- Clientes con poco tiempo en la empresa abandonan más.
- Pagos automáticos reducen la cancelación.
- Cheque electrónico tiene mayor churn.

## Estrategias
- Incentivar contratos de 1 o 2 años.
- Promover pagos automáticos.
- Implementar programas de fidelización temprana.
- Ofrecer paquetes con servicios adicionales.
