# El “Filtro de Calidad”

RSI en Sobreventa vs. Riesgo de Cola Extremo

## 📌Descripción General

Este proyecto implementa un filtro de calidad avanzado para señales técnicas de sobreventa, combinando RSI (momentum) con kurtosis (riesgo de cola).

La idea central es simple pero poderosa:
- no toda acción con RSI < 30 es una oportunidad de rebote.

Algunas están en colapso estructural, y la kurtosis lo delata.

## 📍Insight Clave

- ¿Cuándo una señal clásica de sobreventa es en realidad una trampa mortal?

Un RSI bajo acompañado de kurtosis extremadamente alta indica que:
- los retornos tienen colas gruesas,
- los eventos extremos son frecuentes,
- el riesgo no es técnico, sino fundamental o sistémico.

## 💼Valor de Negocio

- Evita “atrapar cuchillos que caen”.
- Mejora la calidad de estrategias de rebote técnico.
- Reduce drawdowns catastróficos en carteras cuantitativas.

Distingue entre:
- pánico temporal,
- y deterioro irreversible del activo.
- Fundamental para trading sistemático y gestión de riesgo.

Fuentes de Datos
- indicadores_tecnicos
- ticker_id
- fecha
- rsi_14
- kurtosis
- tickers
- ticker_id
- nombre_empresa
- sector

## 🧠Lógica del Análisis

Se toma el estado más reciente de cada acción.

Se filtran acciones con:
- RSI < 30 (sobreventa clásica).

Se aplica el filtro de peligro:
- kurtosis > 7.0
- Se ordenan los resultados por severidad del riesgo de cola.

## 📊Interpretación de Resultados

RSI < 30 + Kurtosis moderada (< 4–5)
→ Sobreventa técnica tradicional.
→ Posible rebote.

RSI < 30 + Kurtosis alta (> 7)
→ Colapso estructural.
→ Alto riesgo de quiebra, fraude o dilución masiva.

Kurtosis extrema persistente
→ El mercado no está exagerando: está anticipando algo serio.

## 🧩Casos de Uso

- Filtro previo a estrategias mean-reversion.
- Protección de carteras long-only.
- Screening de riesgo oculto.
- Trading cuantitativo con control de colas.
- Complemento a análisis fundamental.

## 🚀Posibles Extensiones

- Excluir automáticamente estos activos de estrategias de rebote.
- Analizar persistencia de kurtosis extrema.
- Combinar con volumen anómalo o gaps.
- Usar umbrales dinámicos por sector.
- Integrar con alertas tempranas de distress financiero.

## ✒️Nota Final

El RSI te dice cuándo el mercado está asustado.
La kurtosis te dice si el miedo está justificado.

## 👤Autora
Flavia Hepp Proyecto de SQL aplicó un análisis de riesgo basado en eventos.
Este filtro no busca oportunidades.
Busca evitar errores irreversibles 🛑📉

***
🔪 **RSI < 30… ¿oportunidad de compra o cuchillo cayendo?**

Una de las señales más conocidas del análisis técnico es:

👉 **RSI < 30 = sobreventa → posible rebote**

Pero hay un problema…

No todas las caídas son iguales.

---

📊 En este análisis apliqué un filtro adicional:

* RSI < 30 (sobreventa)
* **Kurtosis > 7** (riesgo extremo de cola)

---

⚠️ ¿Qué significa esto?

👉 RSI bajo → precio cayó fuerte
👉 Kurtosis alta → esa caída **no es normal**

💡 Es una señal de alerta:

* Eventos extremos más frecuentes
* Posible colapso estructural
* Riesgo de noticias negativas (fraude, quiebra, etc.)

---

🚨 Insight clave:
**No todo lo que está sobrevendido está “barato”…
a veces está roto.**

---

🧠 Este es el verdadero “filtro de calidad”:

✔️ Evita atrapar cuchillos cayendo
✔️ Filtra señales falsas de rebote
✔️ Mejora la gestión de riesgo

---

📉 Porque en trading, el objetivo no es solo encontrar oportunidades…
es **evitar las malas**.

---

#Quant #Trading #DataScience #RSI #RiskManagement #Kurtosis #Finanzas
