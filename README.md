
# 🧠 ExcelAnalyzerAgent

**ExcelAnalyzerAgent** es una herramienta interactiva impulsada por inteligencia artificial que permite analizar archivos Excel de forma automatizada, enfocándose especialmente en datos de retail/farmacia. Utiliza el modelo de lenguaje de Groq para responder preguntas sobre los datos, identificar patrones y generar recomendaciones para optimizar el surtido de productos.

## 🚀 Funcionalidades principales

- 📂 Carga interactiva de archivos `.xlsx` o `.xls`.
- 📊 Resumen completo del dataset: estadísticas, columnas, muestras, valores faltantes.
- 🤖 Análisis completo de todos los registros mediante un modelo LLM (por defecto `deepseek-r1-distill-llama-70b`).
- 📌 Optimización automática del surtido con criterios de ventas, margen y rotación.
- 💾 Exportación del análisis a un archivo `.txt`.
- 🖥️ Interfaz por consola para navegación simple y efectiva.

## 🧠 Requisitos

- Python 3.8 o superior
- Una clave API válida de [Groq](https://console.groq.com/)
- Un archivo `.env` con la variable `GROQ_API_KEY`

### Ejemplo de `.env`

```env
GROQ_API_KEY=tu_clave_aqui
```

## 📦 Instalación

1. Cloná el repositorio:

```bash
git clone https://github.com/tu_usuario/ExcelAnalyzerAgent.git
cd ExcelAnalyzerAgent
```

2. Instalá las dependencias:

```bash
pip install -r requirements.txt
```

3. Ejecutá el script:

```bash
python excel_analyzer_agent.py
```

## 📁 Estructura del proyecto

```
.
├── excel_analyzer_agent.py     # Script principal
├── .env                        # Tu clave API (no compartir)
└── README.md                   # Este archivo
```

## 📌 Librerías utilizadas

- [`pandas`](https://pandas.pydata.org/): manejo de datos Excel.
- [`groq`](https://pypi.org/project/groq/): API de modelos LLM de Groq.
- [`dotenv`](https://pypi.org/project/python-dotenv/): manejo de variables de entorno.
- [`tkinter`](https://docs.python.org/3/library/tkinter.html): para selección de archivos y exportación.
- `logging`, `datetime`, `os`, `typing`: utilidades estándar de Python.

## 🧪 Ejemplo de uso

1. Al ejecutar el script, seleccionás un archivo Excel desde una ventana emergente.
2. Elegís una opción del menú (ver resumen, hacer una pregunta, exportar, etc.).
3. El modelo analiza el dataset completo y devuelve un análisis detallado.
4. Podés guardar el resultado como `.txt`.

## 🛡️ Notas de seguridad

Este proyecto utiliza claves API externas. **Nunca compartas tu archivo `.env` ni subas tu clave API a un repositorio público**.

## 📄 Licencia

MIT © [Tu nombre o usuario]
