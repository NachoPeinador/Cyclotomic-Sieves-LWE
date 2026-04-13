# 🐋 Arquitectura Leviatán: Motor Termodinámico de Factorización

[](https://www.google.com/search?q=https://opensource.org/licenses/MIT)
[](https://www.google.com/search?q=https://isocpp.org/)
[](https://www.google.com/search?q=https://www.python.org/)
[](https://www.google.com/search?q=)

**Leviatán** es un motor híbrido (C++/Python) de factorización de enteros masivos y triaje de primalidad. Basado en los principios del Caos Cuántico Aritmético y la fase No Ergódica Extendida (NEE), Leviatán no aplica fuerza bruta ciega, sino que explota la topología del vacío aritmético reduciendo la entropía del espacio de búsqueda mediante restricciones modulares y compresión fractal.

## 📖 Visión General

Los motores de factorización convencionales asumen el espacio de búsqueda como un continuo homogéneo de máxima entropía. Leviatán aplica un diseño termo-computacional anclado en la memoria Caché L1 que aprovecha la "fricción quiral" del espectro de los números primos, operando exclusivamente en los canales permitidos por simetrías modulares.

El motor consta de tres núcleos principales:

  * **Leviatán-Base:** Operador general sobre $\mathbb{Z}/6\mathbb{Z}$. Implementa el método de Fermat modificado con saltos espaciales $x \mathrel{+}= 3$ y artillería ECM (Método de Curva Elíptica) guiada por progresiones asíncronas de Airy.
  * **Leviatán-M (Cazador de Mersenne):** Subsistema balístico de triaje topológico para números de Mersenne ($M_p$). Capaz de descartar candidatos en el rango $p > 137,000,000$ (más de 41 millones de dígitos) en fracciones de segundo evitando el Test de Lucas-Lehmer para compuestos tempranos.
  * **Leviatán-C (Complejo/Ciclotómico):** Extensión topológica para factorizar ideales algebraicos sobre el anillo de enteros de Gauss $\mathbb{Z}[i]$, empleando el primorial atractor $\langle 3(1+i) \rangle$ y curvas elípticas con Multiplicación Compleja (CM).

## 🔬 Fundamentos Físico-Matemáticos

La arquitectura codifica directamente en hardware tres constantes fundamentales derivadas de la termodinámica del vacío aritmético:

1.  **Confinamiento Fractal ($D_2 \approx 0.24338$):** La entropía del criptograma no escala linealmente con sus bits, sino con la dimensión fractal del soporte cuántico, ahorrando hasta un 75% del volumen de búsqueda. En dominios ciclotómicos, se recalibra mediante la Constante de Catalan $G$.
2.  **Acoplamiento Crítico ($\epsilon_c = \pi\sqrt{2}$):** Utilizado para balancear el número de curvas elípticas instanciadas por núcleo sin causar colapso térmico o dispersión estocástica.
3.  **Límite de Chandrasekhar Informativo:** El sistema respeta los primoriales de máxima eficiencia para evitar que la explosión combinatoria de canales ahogue la memoria L1.

## ⚙️ Arquitectura del Sistema

  * **Vanguardia (C++):** Módulos nativos paralelizables orientados a operaciones en memoria L1. Manejo de matrices de bits (bitsets) y aritmética de enteros empaquetados de 64/128 bits.
  * **Orquestador Asíncrono (Python):** Gestiona la logística termodinámica, el pre-filtro de los canales modulares $\mathcal{C}_1$ y $\mathcal{C}_5$, y calcula la entropía efectiva de las oleadas ECM.

## 🚀 Instalación y Compilación

### Requisitos

  * Compilador C++ compatible con C++17 (GCC 9+ o Clang 10+).
  * Python 3.10 o superior.
  * Librerías Python: `numpy`, `scipy` (para herramientas de diagnóstico y notebooks).

### Proceso de compilación

El motor C++ requiere optimizaciones nativas de arquitectura para maximizar el uso de registros y memoria Caché:

```bash
# Clonar el repositorio
git clone https://github.com/TU_USUARIO/Leviatan.git
cd Leviatan

# Compilar los binarios de la Vanguardia C++
g++ -O3 -march=native -mtune=native -std=c++17 src/cpp/leviatan_core.cpp -o bin/leviatan_core
g++ -O3 -march=native -mtune=native -std=c++17 src/cpp/mersenne_triage.cpp -o bin/mersenne_triage
```

## 💻 Uso Básico

El orquestador en Python se encarga de invocar los binarios y administrar los hilos de ejecución.

**1. Factorización de Semiprimos (Leviatán-Base):**

```bash
python main.py factorize --target 114157849 --mode base
```

**2. Triaje de Mersenne (Leviatán-M):**

```bash
python main.py mersenne_triage --range_start 137000000 --k_depth 500000000
```

**3. Factorización en Entornos Ciclotómicos (Leviatán-C):**

```bash
python main.py factorize_complex --norm 100000000000000000000 --ring gauss
```

## 📁 Estructura del Proyecto

```text
Leviatan/
├── bin/                    # Binarios compilados
├── src/
│   ├── cpp/                # Núcleos de Vanguardia (ALU y L1D)
│   │   ├── leviatan_core.cpp
│   │   ├── mersenne_triage.cpp
│   │   └── gauss_ideal_alu.cpp
│   └── python/             # Orquestador Asíncrono y Calibración Fractal
│       ├── orquestador.py
│       ├── ecm_airy.py
│       └── diagnostico.py
├── notebooks/              # Laboratorios Jupyter (Validación de Constantes)
│   ├── Leviatan_Ciclotomico_Lab.ipynb
│   └── Demostracion_Fractal_D2.ipynb
├── main.py                 # Interfaz de Línea de Comandos (CLI)
├── LICENSE
└── README.md
```

## 📚 Referencias Académicas

La base matemática de este código se encuentra detallada en los siguientes manuscritos:

  * Peinador Sala, J. I. (2026). *Explicit Hermitian Hamiltonian for the Riemann Zeros from Modular Arithmetic Quantum Chaos and Multifractality from $\mathbb{Z}/6\mathbb{Z}$*. (Sometido a APS Open Science, JR10006).
  * Peinador Sala, J. I. *Termodinámica de Cribas en Extensiones Ciclotómicas: Funciones L y la Constante de Catalan*. (Manuscrito).

-----
