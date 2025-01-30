# 🚀 LinkedIn Job Scraper 📊

Este repositorio contiene un **web scraper** que extrae información de ofertas de trabajo publicadas en **LinkedIn**, utilizando **BeautifulSoup** y **requests**. El script extrae información clave sobre las vacantes, incluyendo la ubicación, empresa, cargo, requisitos de idioma, habilidades técnicas y blandas, y rango salarial.

---

## 📌 Características

✅ **Búsqueda personalizada** por título de trabajo y ubicación.  
✅ **Extracción de datos clave** como nombre de empresa, ubicación, habilidades requeridas y nivel de inglés.  
✅ **Filtrado automático** de habilidades técnicas, duras y blandas utilizando expresiones regulares.  
✅ **Exportación de datos** a un archivo **CSV** para su posterior análisis.  

---

## 🛠️ Instalación

Para ejecutar este scraper, sigue los siguientes pasos:

### 1️⃣ Clonar el repositorio

```bash
https://github.com/Leonardo-Pantoja/LinkedinJobScrapper.git
cd tu-LinkedinJobScrapper.git
```

## 📄 Uso
Para ejecutar el scraper, edita las variables title y location en el código:
```python
title = "Analista de datos"  # Cargo a buscar
location = "Mexico"          # Ubicación
```

Al finalizar, se generará un archivo job_list.csv con los datos extraídos.

## 📊 Datos extraídos
El scraper extrae la siguiente información de cada oferta de empleo:

| Campo              | Descripción |
|--------------------|-------------|
| `location`        | Ubicación de la oferta |
| `company_name`    | Nombre de la empresa |
| `job_title`       | Cargo del puesto |
| `requires_degree` | Si se requiere un grado académico |
| `english_level`   | Nivel de inglés requerido |
| `technical_skills` | Habilidades técnicas mencionadas en la oferta |
| `hard_skills`     | Habilidades duras detectadas |
| `soft_skills`     | Habilidades blandas detectadas |
| `salary_min`      | Salario mínimo (si está disponible) |
| `job_link`        | Enlace a la publicación en LinkedIn |

## 📌 Notas importantes
⚠️ Este scraper **no utiliza la API** oficial de LinkedIn y puede verse afectado si LinkedIn cambia su estructura HTML.

⚠️ **Evita hacer demasiadas solicitudes en poco tiempo** para no ser bloqueado. Se recomienda agregar pausas (time.sleep()) entre peticiones.

⚠️ Algunas ofertas pueden no incluir toda la información, por lo que es normal encontrar valores No especificado en ciertos campos.
