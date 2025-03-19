# Segmentación de Clientes con la Metodología RFM

## Propósito del Proyecto

Este proyecto tiene como objetivo **segmentar a los clientes** de un conjunto de datos de transacciones utilizando la metodología RFM (Recencia, Frecuencia, Valor Monetario). RFM es una técnica popular en el análisis de datos de clientes, especialmente en marketing y análisis de comportamiento de compra. El proyecto agrupa a los clientes según tres variables clave que reflejan su comportamiento de compra:

1. **Recencia (R)**: Cuánto tiempo ha pasado desde la última compra de un cliente.
2. **Frecuencia (F)**: Cuántas veces un cliente ha realizado compras.
3. **Valor Monetario (M)**: El gasto total de un cliente.

Esta segmentación es útil para personalizar las estrategias de marketing y mejorar la toma de decisiones en cualquier tipo de industria que dependa de sus clientes.

## Datos Utilizados

El conjunto de datos utilizado proviene de un archivo CSV llamado `M30 Online Retail.csv`, que contiene información sobre transacciones en línea de una tienda. Cada fila en el conjunto de datos representa una transacción, con columnas como:

- **INVOICE_NO**: Número de factura.
- **CUSTOMER_ID**: Identificador único de cliente.
- **INVOICE_DATE**: Fecha de la transacción.
- **QUANTITY**: Cantidad de productos comprados.
- **UNIT_PRICE**: Precio unitario del producto.
- **DESCRIPTION**: Descripción del producto.
- **REGION**: Región de la transacción.

### Pasos realizados con los datos

1. **Limpieza de datos**: Eliminación de duplicados y valores nulos.
2. **Análisis exploratorio de datos**: Análisis de las variables como las cantidades de productos comprados y los precios unitarios.
3. **Cálculos adicionales**: Cálculo del gasto total por cliente y la recencia de la última compra.

## Técnicas Aplicadas

1. **Limpieza de datos**: Eliminación de registros duplicados y manejo de valores nulos en las fechas de las transacciones.
   
2. **Cálculo de Métricas RFM**:
   - **Recencia (R)**: Calculamos la diferencia en días entre la última compra de cada cliente y la fecha de la última transacción.
   - **Frecuencia (F)**: Calculamos el número de compras realizadas por cada cliente.
   - **Valor Monetario (M)**: Calculamos el gasto total de cada cliente, multiplicando la cantidad de productos comprados por su precio unitario.

3. **Normalización de datos**: Se estandarizaron los datos RFM utilizando `StandardScaler` para asegurar que las métricas tuvieran la misma escala.

4. **Algoritmo de K-Means**: Se utilizó el algoritmo de K-Means para realizar la segmentación de los clientes en varios grupos basados en sus características de recencia, frecuencia y valor monetario.

5. **Análisis de Componentes Principales (PCA)**: PCA se usó para reducir la dimensionalidad y visualizar los clústeres de clientes en un espacio de dos dimensiones.

6. **Visualización**: Se crearon varias visualizaciones como histogramas y gráficos de dispersión para analizar las distribuciones y patrones en los datos de recencia, frecuencia y valor monetario.

7. **Segmentación Final**: Después de realizar la segmentación, se asignó una categoría a cada cliente (bajo, promedio, potencial, alto valor) en función de su puntaje en las tres métricas.

## Conclusiones

1. **Segmentación de clientes**: El análisis mostró que los clientes pueden ser segmentados efectivamente según su comportamiento de compra, lo que proporciona una base para personalizar las estrategias de marketing.

2. **Distribuciones de variables**: Las visualizaciones de las distribuciones de recencia, frecuencia y valor monetario proporcionaron información clave sobre cómo los clientes varían en términos de actividad y gasto.

3. **Rendimiento de K-Means**: El uso de K-Means ayudó a identificar distintos segmentos de clientes, lo que puede ser útil para realizar campañas específicas para cada grupo.

4. **Clasificación de clientes**: Se clasificó a los clientes en diferentes categorías de valor, lo que permite a las empresas focalizar sus recursos y esfuerzos en los clientes con mayor potencial de generar ingresos.

5. **Mejoras posibles**: Se podrían realizar mejoras en la segmentación utilizando algoritmos más avanzados o incorporando variables adicionales, como el tipo de producto comprado, el comportamiento en redes sociales o la ubicación geográfica.

## Requisitos
Para ejecutar este proyecto, se necesitan las siguientes librerías de Python:
- **pandas**
- **numpy**
- **matplotlib**
- **seaborn**
- **scikit-learn**

## Resultados
![image](https://github.com/user-attachments/assets/ae32e5da-a3e1-4e43-b729-a52344d84bb0)
![image](https://github.com/user-attachments/assets/c8ca44e0-f651-4d78-8b20-6989418ff3c4)
![image](https://github.com/user-attachments/assets/aa81c7a3-48bf-45f8-98f2-a34d9616977d)
![image](https://github.com/user-attachments/assets/6794e9e8-c79a-474a-8af1-f3543453e054)
![image](https://github.com/user-attachments/assets/f75c9966-db52-4441-854d-a5ba317f700f)
![image](https://github.com/user-attachments/assets/4d2b6459-634c-4826-b06b-484d320caefd)
![image](https://github.com/user-attachments/assets/5803d52f-5a5c-4777-9ee3-8422cb6df5bb)
![image](https://github.com/user-attachments/assets/3dad6bea-c72c-4c87-aaf7-60a14b4e6fac)
![image](https://github.com/user-attachments/assets/c97f4860-a2d4-44e4-9c50-851d4ee7f8b3)
![image](https://github.com/user-attachments/assets/49d81c86-8609-4eed-ac38-b0ec75580238)
![image](https://github.com/user-attachments/assets/bbb2b766-ed81-41a8-905e-055e867a8514)
![image](https://github.com/user-attachments/assets/e251be60-3af0-48fc-8d33-a9915e5422d8)
![image](https://github.com/user-attachments/assets/85336c7e-adea-4e18-9371-42ec3e45dd49)
![image](https://github.com/user-attachments/assets/b92f7597-993f-4339-b872-ebf7339060cf)
![image](https://github.com/user-attachments/assets/9b8ed8d3-6aaa-4b59-89dd-084aebb8f43b)



