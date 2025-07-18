# 📊 Proyecto Sprint 5 – Análisis de Tarifas de Megaline

Este proyecto consiste en analizar el comportamiento de los usuarios de la empresa de telecomunicaciones **Megaline**, con el objetivo de identificar patrones de consumo, calcular ingresos mensuales y evaluar la rentabilidad de dos planes tarifarios: **Surf** y **Ultimate**.

---

## 🧾 Descripción de las tarifas

Megaline redondea los segundos a minutos y los megabytes a gigabytes.  
- **Llamadas**: cada llamada se redondea individualmente (1 segundo = 1 minuto).  
- **Internet**: el total mensual se redondea hacia arriba (1025 MB = 2 GB).

### 📦 Plan Surf
- Pago mensual: $20  
- Incluye: 500 minutos, 50 SMS, 15 GB  
- Exceso:  
  - Minuto adicional: $0.03  
  - SMS adicional: $0.03  
  - GB adicional: $10  

### 📦 Plan Ultimate
- Pago mensual: $70  
- Incluye: 3000 minutos, 1000 SMS, 30 GB  
- Exceso:  
  - Minuto adicional: $0.01  
  - SMS adicional: $0.01  
  - GB adicional: $7  

---

## 🗃️ Diccionario de datos

El proyecto utiliza cinco tablas:

- **users**: información personal y plan contratado  
- **calls**: duración y fecha de llamadas  
- **messages**: cantidad y fecha de SMS  
- **internet**: volumen de datos por sesión  
- **plans**: detalles de cada tarifa

---

## 🧪 Objetivos del análisis

1. **Preparar los datos**: convertir tipos, limpiar errores y agrupar por usuario y mes.
2. **Calcular ingresos mensuales**: según uso y límites del plan.
3. **Analizar comportamiento del cliente**: minutos, SMS y datos por mes.
4. **Visualizar distribuciones**: histogramas, medias, varianzas y desviaciones estándar.
5. **Probar hipótesis**:
   - ¿Los ingresos promedio difieren entre los planes Surf y Ultimate?
   - ¿Los ingresos promedio en el área NY-NJ son diferentes al resto del país?

---

## 📈 Herramientas utilizadas

- `pandas` para manipulación de datos  
- `matplotlib` y `seaborn` para visualización  
- `scipy.stats.ttest_ind` para pruebas estadísticas  
- Expresiones regulares para segmentación de datos

---

## ✅ Resultados

- Se identificaron diferencias significativas en los ingresos entre los planes tarifarios.
- El área NY-NJ mostró un comportamiento distinto en consumo y rentabilidad.
- Se aplicaron pruebas estadísticas con un valor alfa definido por el analista.

---

## 🧠 Conclusión

Este proyecto demuestra cómo aplicar análisis exploratorio, limpieza de datos y pruebas de hipótesis para tomar decisiones informadas sobre estrategias tarifarias. Refuerza habilidades clave en Python, análisis estadístico y visualización de datos.
