import React, { useState } from 'react';
import { Globe2 } from 'lucide-react';

const BikeRentalPage = () => {
  const [language, setLanguage] = useState('spanish');

  const content = {
    spanish: {
      title: 'Predicción de Demanda de Alquiler de Bicicletas 🚴‍♂️📊',
      sections: [
        {
          title: '📝 Descripción del Proyecto',
          content: 'Este proyecto se centra en predecir la demanda de alquiler de bicicletas utilizando modelos de regresión. El objetivo es predecir el número de bicicletas alquiladas en función de datos meteorológicos y estacionales.'
        },
        {
          title: '🛠️ Tecnologías Utilizadas',
          items: [
            { title: 'Python', desc: 'El lenguaje de programación principal utilizado para el análisis de datos y la construcción de modelos.' },
            { title: 'Pandas', desc: 'Para la manipulación y análisis de datos.' },
            { title: 'NumPy', desc: 'Para cálculos numéricos.' },
            { title: 'Matplotlib & Seaborn', desc: 'Para la visualización de datos.' },
            { title: 'Scikit-learn', desc: 'Para modelos de aprendizaje automático y métricas de evaluación.' },
            { title: 'XGBoost', desc: 'Para modelos avanzados de regresión.' },
            { title: 'Statsmodels', desc: 'Para análisis estadístico y cálculo del factor de inflación de la varianza (VIF).' }
          ]
        }
      ]
    },
    english: {
      title: 'Bike Rental Demand Prediction 🚴‍♂️📊',
      sections: [
        {
          title: '📝 Project Overview',
          content: 'This project focuses on predicting bike rental demand using regression models. The goal is to forecast the number of rented bikes based on weather and seasonal data.'
        },
        {
          title: '🛠️ Technologies Used',
          items: [
            { title: 'Python', desc: 'The primary programming language used for data analysis and model building.' },
            { title: 'Pandas', desc: 'For data manipulation and analysis.' },
            { title: 'NumPy', desc: 'For numerical computations.' },
            { title: 'Matplotlib & Seaborn', desc: 'For data visualization.' },
            { title: 'Scikit-learn', desc: 'For machine learning models and evaluation metrics.' },
            { title: 'XGBoost', desc: 'For advanced regression modeling.' },
            { title: 'Statsmodels', desc: 'For statistical analysis and variance inflation factor (VIF) calculation.' }
          ]
        }
      ]
    }
  };

  return (
    <div className="min-h-screen bg-gray-50">
      {/* Header */}
      <header className="bg-blue-900 text-white py-6 px-4">
        <div className="max-w-4xl mx-auto">
          <h1 className="text-3xl font-bold text-center mb-6">
            {content[language].title}
          </h1>
          
          {/* Language Toggle */}
          <div className="flex justify-center gap-4">
            <button
              onClick={() => setLanguage('spanish')}
              className={`px-4 py-2 rounded-lg flex items-center gap-2 ${
                language === 'spanish' 
                  ? 'bg-yellow-500 text-blue-900 font-bold'
                  : 'bg-blue-800 hover:bg-blue-700'
              }`}
            >
              <Globe2 size={20} />
              Español
            </button>
            <button
              onClick={() => setLanguage('english')}
              className={`px-4 py-2 rounded-lg flex items-center gap-2 ${
                language === 'english'
                  ? 'bg-yellow-500 text-blue-900 font-bold'
                  : 'bg-blue-800 hover:bg-blue-700'
              }`}
            >
              <Globe2 size={20} />
              English
            </button>
          </div>
        </div>
      </header>

      {/* Main Content */}
      <main className="max-w-4xl mx-auto py-8 px-4">
        {content[language].sections.map((section, index) => (
          <section key={index} className="mb-12">
            <h2 className="text-2xl font-bold mb-4 text-blue-900">
              {section.title}
            </h2>
            
            {section.content && (
              <p className="text-gray-700 leading-relaxed mb-6">
                {section.content}
              </p>
            )}
            
            {section.items && (
              <ul className="space-y-4">
                {section.items.map((item, i) => (
                  <li key={i} className="bg-white p-4 rounded-lg shadow-sm">
                    <h3 className="font-bold text-blue-900 mb-1">
                      {item.title}
                    </h3>
                    <p className="text-gray-600">{item.desc}</p>
                  </li>
                ))}
              </ul>
            )}
          </section>
        ))}
      </main>
    </div>
  );
};

export default BikeRentalPage;
