# Predicción del abandono de clientes 🤖

![Predicción del abandono de clientes](Images/Portada-abandono-clientes.png)

Una empresa de telecomunicaciones (Vodafone) desea estimar la probabilidad de que un cliente abandone la compañía. Este proyecto tiene como objetivo desarrollar un modelo de clasificación capaz de predecir si un cliente abandonará el servicio (**churn**) o permanecerá en la empresa.

## Descripción General del Proyecto

En este proyecto se emplean técnicas de **Machine Learning Supervisado (Clasificación)** para analizar la importancia de la analítica de abandono de clientes (*churn analytics*) como una herramienta estratégica para las empresas de telecomunicaciones. El propósito es identificar de manera proactiva los principales factores de riesgo asociados al abandono de clientes, optimizar las estrategias de retención y fortalecer las relaciones a largo plazo con los usuarios.

El proyecto sigue la metodología **CRISP-DM (Cross-Industry Standard Process for Data Mining)**, un marco de trabajo ampliamente utilizado en proyectos de minería de datos y ciencia de datos, para explorar, procesar y analizar el fenómeno del abandono de clientes dentro de la red de servicios de Vodafone.

El modelo predictivo de abandono de clientes constituye una solución basada en datos diseñada para abordar el desafío constante de la pérdida de clientes en industrias basadas en suscripciones. Su objetivo es identificar a los clientes con mayor riesgo de abandonar el servicio, permitiendo a la empresa implementar acciones preventivas y desarrollar estrategias de retención personalizadas que contribuyan a mejorar la fidelización de los clientes.

## Tabla de Contenidos 📖
- [Descripción del Proyecto](#project-overview)
- [Enlaces del Proyecto](#project-links-link)
- [Herramientas Utilizadas en el Proyecto](#some-tools-used-for-the-project-toolbox)
- [Conjunto de Datos](#dataset-floppy_disk)
- [Proceso](#process)
- [Rendimiento del Modelo](#model-performance-accuracy-bar_chart)
- [Dashboard](#power-bi-dashboard-tv)
- [Conclusiones y Recomendaciones](#conclusion-and-recommendation)
- [Cómo Utilizar este Repositorio](#how-to-use-this-repository-monocle_face)
- [Author](#author-writing_hand)

##  Herramientas Utilizadas en el Proyecto :toolbox:
<p align="left">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" alt="vscode" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original-wordmark.svg" alt="pandas" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" alt="numpy" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="python" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original-wordmark.svg" alt="jupyter" width="45" height="45"/>
</p>


## Dataset :floppy_disk:

**Descripción de variables de las bases de datos**
| **Nombre de la Variable** | **Descripción** | **Tipo de Dato** |
|---------------------------|-----------------|------------------|
| `customerID` | Contiene el identificador único del cliente. | Categórico |
| `gender` | Indica si el cliente es mujer o hombre. | Categórico |
| `SeniorCitizen` | Indica si el cliente es un adulto mayor o no (1 = Sí, 0 = No). | Numérico (entero) |
| `Partner` | Indica si el cliente tiene pareja (Sí, No). | Categórico |
| `Dependents` | Indica si el cliente tiene dependientes (Sí, No). | Categórico |
| `tenure` | Número de meses que el cliente ha permanecido en la empresa. | Numérico (entero) |
| `PhoneService` | Indica si el cliente cuenta con servicio telefónico (Sí, No). | Categórico |
| `MultipleLines` | Indica si el cliente tiene múltiples líneas telefónicas (Sí, No, Sin servicio telefónico). | Categórico |
| `InternetService` | Tipo de servicio de Internet del cliente (DSL, Fibra óptica, Sin servicio). | Categórico |
| `OnlineSecurity` | Indica si el cliente cuenta con servicio de seguridad en línea (Sí, No, Sin servicio de Internet). | Categórico |
| `OnlineBackup` | Indica si el cliente cuenta con servicio de respaldo en línea (Sí, No, Sin servicio de Internet). | Categórico |
| `DeviceProtection` | Indica si el cliente cuenta con servicio de protección de dispositivos (Sí, No, Sin servicio de Internet). | Categórico |
| `TechSupport` | Indica si el cliente cuenta con soporte técnico (Sí, No, Sin servicio de Internet). | Categórico |
| `StreamingTV` | Indica si el cliente cuenta con servicio de televisión por streaming (Sí, No, Sin servicio de Internet). | Categórico |
| `StreamingMovies` | Indica si el cliente cuenta con servicio de películas por streaming (Sí, No, Sin servicio de Internet). | Categórico |
| `Contract` | Tipo de contrato del cliente (Mensual, Un año, Dos años). | Categórico |
| `PaperlessBilling` | Indica si el cliente utiliza facturación electrónica (Sí, No). | Categórico |
| `PaymentMethod` | Método de pago del cliente (Cheque electrónico, Cheque enviado por correo, Transferencia bancaria, Tarjeta de crédito). | Categórico |
| `MonthlyCharges` | Monto cobrado mensualmente al cliente. | Numérico (decimal) |
| `TotalCharges` | Monto total cobrado al cliente. | Objeto (`object`) |
| `Churn` | Indica si el cliente abandonó el servicio o no (Sí, No). | Categórico |

## Proceso

- Extraer datos de múltiples fuentes, incluyendo una base de datos remota en SQL Server.

- Formular la hipótesis y definir las preguntas analíticas que se buscarán responder.

- Realizar el preprocesamiento y la limpieza de los datos, así como el Análisis Exploratorio de Datos (EDA), incluyendo análisis univariado, bivariado y multivariado.

- Responder las preguntas analíticas mediante visualizaciones.

- Desarrollar y desplegar visualizaciones interactivas en Power BI.

- Balancear el conjunto de datos utilizando el algoritmo **SMOTE** para sobremuestreo (*oversampling*).

- Realizar ingeniería de características (*Feature Engineering*) y escalamiento de variables.

- Entrenar y evaluar modelos de aprendizaje automático.

- Optimizar los modelos mediante el ajuste de hiperparámetros (*Hyperparameter Tuning*).

- Realizar pruebas de predicción e implementar mejoras en el modelo.

- Presentar las conclusiones y documentar el proyecto mediante la elaboración de un artículo o informe técnico.

## Rendimiento del Modelo :bar_chart:

<table>
    <tr>
        <th>Precisión de los Modelos Entrenados</th>
    </tr>
    <tr>
        <td><img src="Screenshots\Model_Performance_Accuracy.png"/></td>
    </tr>
</table>

## Conclusiones y Recomendaciones

- El número de meses que el cliente ha permanecido en la empresa (**tenure**) y el tipo de contrato del cliente (**Contract**) son las variables más importantes y presentan la mayor relación con el abandono de clientes (**Churn**).

- Vodafone debería fortalecer la experiencia del cliente durante los primeros meses de permanencia. El análisis muestra que entre los **5 y 10 primeros meses** los clientes presentan una mayor probabilidad de abandonar el servicio, lo que indica que la experiencia inicial es determinante. Mejorar el proceso de incorporación (*onboarding*), la calidad del servicio y brindar un soporte técnico oportuno durante este periodo puede incrementar la satisfacción y la fidelización de los clientes.

- Vodafone debería promover contratos de mayor duración. Los resultados muestran que los clientes con contratos **mensuales (Month-to-Month)** presentan una tasa de abandono significativamente mayor que aquellos con contratos de **uno o dos años**. Incentivar la contratación de planes de mayor duración mediante beneficios, promociones y un mejor soporte técnico podría reducir la tasa de abandono y fortalecer el compromiso de los clientes con la empresa.

- El ajuste de hiperparámetros (*Hyperparameter Tuning*) no siempre produce mejoras significativas en el rendimiento de los modelos.

- Utilizando una partición de **80 % para entrenamiento y 20 % para evaluación**, el modelo **Random Forest** alcanzó una precisión aproximada del **86 %** después del ajuste de hiperparámetros.

- Los métodos de **ensamble (Ensemble Methods)** presentan un mejor desempeño en tareas de clasificación en comparación con los modelos basados en un único clasificador.

## Cómo utilizar este repositorio :monocle_face:

Es necesario tener [`Python 3`](https://www.python.org/) instalado en el sistema. Posteriormente, puede clonar este repositorio y ubicarse en el directorio `root :: repository_name> ...`

1. Clonar este repositorio: `git clone https://github.com/CarloEduardo/05-Prediccion-de-Abandono-de-Clientes.git`
2. En su entorno de desarrollo (IDE), crear un entorno virtual e instalar las dependencias necesarias para ejecutar el proyecto:

- Windows:       
        python -m venv venv; 
        venv\Scripts\activate; 
        python -m pip install -q --upgrade pip; 
        python -m pip install -qr requirements.txt  

- Linux & MacOs:
        python3 -m venv venv; 
        source venv/bin/activate; 
        python -m pip install -q --upgrade pip; 
        python -m pip install -qr requirements.txt  

Los dos comandos extensos tienen la misma estructura: encadenan varias instrucciones utilizando el símbolo `;`. No obstante, también pueden ejecutarse manualmente una por una.

- **Crear un entorno virtual de Python**, el cual permitirá aislar las bibliotecas utilizadas en el proyecto y evitar conflictos con otras instalaciones.
- **Activar el entorno virtual**, de modo que el intérprete de Python y las bibliotecas utilizadas correspondan únicamente a dicho entorno.
- **Actualizar Pip**, el gestor de paquetes de Python, para disponer de la versión más reciente y garantizar una correcta instalación de las dependencias.
- **Instalar las bibliotecas requeridas**, especificadas en el archivo `requirements.txt`, para que puedan importarse correctamente tanto en los scripts de Python como en los notebooks de Jupyter.

**Nota:** Si utiliza **macOS** y experimenta problemas durante la instalación, se recomienda instalar `Xcode`.

3. Explorar el notebook de Jupyter para conocer el procedimiento completo y la ejecución del código.
4. Revisar el panel de Power BI para interactuar con las visualizaciones desarrolladas.
5. Leer el artículo publicado para obtener una comprensión más detallada del proyecto y de los resultados obtenidos.

## Autor :writing_hand:
Carlos Eduardo Torres Garcia

<a href="https://www.linkedin.com/in/carlo4-eduardo-torres-garcia/"><img align="left" src="https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white" alt="Carlos Eduardo Torres Garcia | LinkedIn"/></a>

---
