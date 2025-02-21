<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bike Rental Demand Prediction 🚴‍♂️📊</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        #header {
            background-color: #1b3652;
            color: white;
            padding: 10px;
            text-align: center;
        }
        #lang-buttons {
            margin: 10px 0;
            text-align: center;
        }
        #lang-buttons button {
            padding: 10px 20px;
            margin: 0 10px;
            cursor: pointer;
            background-color: #f5b31d;
            border: none;
            font-size: 16px;
        }
        #content {
            padding: 20px;
            line-height: 1.6;
        }
        #english, #spanish {
            display: none;
        }
    </style>
</head>
<body>

<div id="header">
    <h1>Bike Rental Demand Prediction 🚴‍♂️📊</h1>
</div>

<div id="lang-buttons">
    <button onclick="showLanguage('spanish')">Español</button>
    <button onclick="showLanguage('english')">English</button>
</div>

<div id="content">
    <div id="spanish">
        <h2>📝 Descripción del Proyecto</h2>
        <p>Este proyecto se centra en predecir la demanda de alquiler de bicicletas utilizando modelos de regresión. El objetivo es predecir el número de bicicletas alquiladas en función de datos meteorológicos y estacionales. El proyecto incluye la carga de datos, limpieza, análisis exploratorio de datos (EDA) y la aplicación de varios modelos de aprendizaje automático para predecir la demanda de alquiler de bicicletas.</p>

        <h2>🛠️ Tecnologías Utilizadas</h2>
        <ul>
            <li><strong>Python</strong>: El lenguaje de programación principal utilizado para el análisis de datos y la construcción de modelos.</li>
            <li><strong>Pandas</strong>: Para la manipulación y análisis de datos.</li>
            <li><strong>NumPy</strong>: Para cálculos numéricos.</li>
            <li><strong>Matplotlib & Seaborn</strong>: Para la visualización de datos.</li>
            <li><strong>Scikit-learn</strong>: Para modelos de aprendizaje automático y métricas de evaluación.</li>
            <li><strong>XGBoost</strong>: Para modelos avanzados de regresión.</li>
            <li><strong>Statsmodels</strong>: Para análisis estadístico y cálculo del factor de inflación de la varianza (VIF).</li>
        </ul>

        <h2>📂 Estructura del Proyecto</h2>
        <ul>
            <li><strong>Carga y Visión General de los Datos</strong>: Cargar el conjunto de datos y realizar una exploración inicial.</li>
            <li><strong>Limpieza de Datos</strong>: Manejo de valores faltantes, variables categóricas y ingeniería de características.</li>
            <li><strong>Análisis Exploratorio de Datos (EDA)</strong>: Análisis de tendencias y correlaciones entre variables.</li>
            <li><strong>Construcción de Modelos</strong>: Aplicación de varios modelos de regresión para predecir la demanda de alquiler de bicicletas.</li>
            <li><strong>Evaluación de Modelos</strong>: Uso de métricas como Error Absoluto Medio (MAE), Error Cuadrático Medio (MSE) y R-cuadrado (R²) para evaluar el rendimiento de los modelos.</li>
        </ul>

        <h2>🚀 Características Principales</h2>
        <ul>
            <li><strong>Limpieza de Datos</strong>: Manejo exhaustivo de valores faltantes y datos categóricos.</li>
            <li><strong>EDA</strong>: Visualizaciones detalladas para comprender tendencias y relaciones en los datos.</li>
            <li><strong>Modelado</strong>: Aplicación de múltiples modelos de regresión, incluyendo Regresión Lineal, Bosques Aleatorios, Gradient Boosting y XGBoost.</li>
            <li><strong>Optimización de Hiperparámetros</strong>: Uso de RandomizedSearchCV para optimizar los parámetros de los modelos.</li>
        </ul>

        <h2>📊 Resultados</h2>
        <p>El proyecto demuestra la efectividad de diferentes modelos de regresión en la predicción de la demanda de alquiler de bicicletas. El modelo con mejor rendimiento se selecciona en función de las métricas de evaluación, proporcionando información sobre los factores que influyen en los alquileres de bicicletas.</p>

        <h2>📄 Estructura del Repositorio</h2>
        <ul>
            <li><strong>bike_analysis.ipynb</strong>: Cuaderno de Jupyter que contiene el análisis completo y el código.</li>
            <li><strong>data/day.csv</strong>: Conjunto de datos utilizado para el análisis.</li>
            <li><strong>README.md</strong>: Este archivo, que proporciona una visión general del proyecto.</li>
        </ul>

        <h2>📜 Licencia</h2>
        <p>Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.</p>

        <h2>🙏 Agradecimientos</h2>
        <p>Un agradecimiento especial a la comunidad de código abierto por proporcionar las herramientas y bibliotecas utilizadas en este proyecto.</p>
        <p>Inspiración y orientación de varios recursos y tutoriales en línea.</p>
    </div>

    <div id="english">
        <h2>📝 Project Overview</h2>
        <p>This project focuses on predicting bike rental demand using regression models. The goal is to forecast the number of rented bikes based on weather and seasonal data. The project involves data loading, cleaning, exploratory data analysis (EDA), and the application of various machine learning models to predict bike rental counts.</p>

        <h2>🛠️ Technologies Used</h2>
        <ul>
            <li><strong>Python</strong>: The primary programming language used for data analysis and model building.</li>
            <li><strong>Pandas</strong>: For data manipulation and analysis.</li>
            <li><strong>NumPy</strong>: For numerical computations.</li>
            <li><strong>Matplotlib & Seaborn</strong>: For data visualization.</li>
            <li><strong>Scikit-learn</strong>: For machine learning models and evaluation metrics.</li>
            <li><strong>XGBoost</strong>: For advanced regression modeling.</li>
            <li><strong>Statsmodels</strong>: For statistical analysis and variance inflation factor (VIF) calculation.</li>
        </ul>

        <h2>📂 Project Structure</h2>
        <ul>
            <li><strong>Data Loading & Overview</strong>: Load the dataset and perform an initial exploration.</li>
            <li><strong>Data Cleaning</strong>: Handle missing values, categorical variables, and feature engineering.</li>
            <li><strong>Exploratory Data Analysis (EDA)</strong>: Analyze trends and correlations between variables.</li>
            <li><strong>Model Building</strong>: Apply various regression models to predict bike rental demand.</li>
            <li><strong>Model Evaluation</strong>: Use metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²) to evaluate model performance.</li>
        </ul>

        <h2>🚀 Key Features</h2>
        <ul>
            <li><strong>Data Cleaning</strong>: Comprehensive handling of missing values and categorical data.</li>
            <li><strong>EDA</strong>: Detailed visualizations to understand data trends and relationships.</li>
            <li><strong>Modeling</strong>: Application of multiple regression models including Linear Regression, Random Forest, Gradient Boosting, and XGBoost.</li>
            <li><strong>Hyperparameter Tuning</strong>: Use of RandomizedSearchCV for optimizing model parameters.</li>
        </ul>

        <h2>📊 Results</h2>
        <p>The project demonstrates the effectiveness of different regression models in predicting bike rental demand. The best-performing model is selected based on evaluation metrics, providing insights into the factors influencing bike rentals.</p>

        <h2>📄 Repository Structure</h2>
        <ul>
            <li><strong>bike_analysis.ipynb</strong>: Jupyter notebook containing the complete analysis and code.</li>
            <li><strong>data/day.csv</strong>: Dataset used for the analysis.</li>
            <li><strong>README.md</strong>: This file, providing an overview of the project.</li>
        </ul>

        <h2>📜 License</h2>
        <p>This project is licensed under the MIT License. See the LICENSE file for details.</p>

        <h2>🙏 Acknowledgments</h2>
        <p>Special thanks to the open-source community for providing the tools and libraries used in this project.</p>
        <p>Inspiration and guidance from various online resources and tutorials.</p>
    </div>
</div>

<script>
    function showLanguage(language) {
        if(language === 'spanish') {
            document.getElementById('spanish').style.display = 'block';
            document.getElementById('english').style.display = 'none';
        } else if(language === 'english') {
            document.getElementById('spanish').style.display = 'none';
            document.getElementById('english').style.display = 'block';
        }
    }

    // Default language
    showLanguage('spanish');
</script>

</body>
</html>
