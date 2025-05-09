Streamlit Redaction Improver
Mostrar imagen
Descripción
Streamlit Redaction Improver es una aplicación web que utiliza inteligencia artificial para mejorar la calidad y estructura de textos redactados. Esta herramienta permite a los usuarios subir documentos o ingresar texto directamente para ser procesado, analizado y mejorado mediante modelos avanzados de procesamiento de lenguaje natural (NLP).
Características principales

Mejora de redacción: Optimiza la claridad, coherencia y estructura de textos
Análisis de contenido: Identifica problemas comunes como redundancias, inconsistencias o lenguaje impreciso
Interfaz amigable: Desarrollada con Streamlit para una experiencia intuitiva
Soporte para múltiples formatos: Procesa texto plano y documentos (PDF, DOCX, etc.)
Personalización: Opciones para ajustar el nivel y tipo de mejoras aplicadas
Análisis comparativo: Visualización lado a lado del texto original y mejorado


Instalación
Requisitos previos

Python 3.8+
Pip (gestor de paquetes de Python)
Cuenta en OpenAI o proveedor compatible para acceder a las APIs de IA

Pasos de instalación

Clonar el repositorio

bashgit clone https://github.com/arklon1975/streamlit-redaction-improver1.git
cd streamlit-redaction-improver1

Crear y activar un entorno virtual (opcional pero recomendado)

bashpython -m venv venv
# En Windows
venv\Scripts\activate
# En macOS/Linux
source venv/bin/activate

Instalar dependencias

bashpip install -r requirements.txt

Configurar variables de entorno

Crea un archivo .env en el directorio raíz con el siguiente contenido:
OPENAI_API_KEY=tu_clave_api_aquí
Uso

Iniciar la aplicación

bashstreamlit run app.py

Acceder a la interfaz web

Abre tu navegador y visita la dirección mostrada en la terminal (generalmente http://localhost:8501).

Utilizar la aplicación


Sube un documento o ingresa texto directamente
Configura los parámetros de mejora según tus necesidades
Haz clic en "Mejorar texto" y espera los resultados
Compara y descarga el texto mejorado

Estructura del proyecto
streamlit-redaction-improver1/
├── app.py                      # Aplicación principal de Streamlit
├── components/                 # Componentes de la interfaz
│   ├── sidebar.py              # Componentes de la barra lateral
│   ├── text_input.py           # Componentes para entrada de texto
│   └── results_display.py      # Visualización de resultados
├── services/                   # Lógica de servicios
│   ├── ai_service.py           # Integración con APIs de IA
│   ├── text_processor.py       # Procesamiento de texto
│   └── document_handler.py     # Manejo de documentos
├── utils/                      # Utilidades
│   ├── text_analytics.py       # Análisis de texto
│   └── formatters.py           # Formato y presentación
├── assets/                     # Recursos estáticos
│   ├── logo.png                # Logo de la aplicación
│   └── demo.gif                # Demostración animada
├── requirements.txt            # Dependencias del proyecto
├── .env                        # Variables de entorno (no incluir en git)
└── README.md                   # Este archivo
Tecnologías utilizadas

Streamlit: Framework para desarrollo de aplicaciones web en Python
LangChain: Framework para aplicaciones con LLMs
OpenAI API: Motor de IA para procesamiento y mejora de texto
PyPDF2: Biblioteca para manipulación de PDFs
python-docx: Biblioteca para manipulación de documentos DOCX
spaCy: Biblioteca de NLP para análisis lingüístico

Configuración avanzada
Parámetros personalizables
La aplicación permite configurar diversos parámetros para ajustar las mejoras:

Nivel de formalidad: Ajusta el tono desde coloquial hasta académico
Enfoque de mejora: Prioriza claridad, concisión o persuasión
Conservación de estilo: Determina cuánto del estilo original preservar
Idioma objetivo: Optimiza para un idioma o región específica

Estos parámetros se pueden configurar desde la barra lateral de la aplicación.
Ejemplos de uso
Mejora de un correo profesional
Sube un borrador de correo electrónico y selecciona "Formal" como nivel de formalidad para obtener una versión pulida y profesional.
Simplificación de texto técnico
Ingresa un texto técnico complejo y selecciona "Alta" en la opción de simplificación para hacerlo más accesible.
Preparación de contenido académico
Sube un borrador de ensayo académico y selecciona la opción "Académico" para mejorar la estructura y el lenguaje conforme a estándares académicos.
Contribución
Las contribuciones son bienvenidas. Por favor, sigue estos pasos:

Haz fork del repositorio
Crea una rama para tu funcionalidad (git checkout -b feature/amazing-feature)
Haz commit de tus cambios (git commit -m 'Add some amazing feature')
Haz push a la rama (git push origin feature/amazing-feature)
Abre un Pull Request

Guía de estilo

Sigue la convención PEP 8 para el código Python
Incluye docstrings para funciones y clases
Mantén la funcionalidad modular para facilitar las pruebas

Licencia
Este proyecto está licenciado bajo MIT License.
Contacto
Creado por arklon1975
