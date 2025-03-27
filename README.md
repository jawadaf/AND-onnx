# 🧠 Model Transfer i Java Spring med ONNX

Dette projekt demonstrerer, hvordan man kan overføre (transferere) en trænet machine learning-model fra Python (TensorFlow) til Java via ONNX-format, og integrere den i en webapplikation udviklet med Spring Boot. Formålet med projektet er at vise min evne til at kombinere kunstig intelligens med Java-udvikling i praksis.

## 🔧 Teknologier brugt

- Java 17
- Spring Boot
- ONNX Runtime (Java API)
- TensorFlow (Python)
- tf2onnx (Python → ONNX eksport)
- Thymeleaf (HTML-rendering)
- Maven

## 📌 Funktionalitet

Projektet består af to dele:

### ✅ 1. AND-gate forudsigelse
- En simpel model, trænet i Python med TensorFlow, til at simulere AND-logik.
- Eksporteret som `.onnx`-fil.
- Brugt i Java til at lave forudsigelser via ONNX Runtime og vise resultatet i en HTML-side.

➡️ Prøv det på `/numbers` i applikationen.

### 🏦 2. Bankdata-model med normalisering
- En mere kompleks model med 13 inputfelter og indbygget normaliseringslag.
- Inputdata bliver omformet og sendt til modellen.
- Modellen returnerer en sandsynlighed for et givent udfald (f.eks. kundens respons).
  
➡️ Prøv det på `/bank` i applikationen.

## 💼 Hvad jeg har lært og demonstreret

- Forståelse for hvordan machine learning-modeller kan eksporteres og genbruges i forskellige miljøer.
- Brug af ONNX til platformuafhængig modelinference.
- Udvikling af webapplikation i Spring Boot med brugervenlige formularer.
- Praktisk viden om datastrukturering og transformation (fx reshaping og standardisering).
- Evne til at forbinde frontend, backend og ML-inference i én løsning.

## ▶️ Sådan kører du projektet

1. Klon repository:
   ```bash
   git clone https://github.com/jawadaf/AND-onnx.git
   cd AND-onnx
