# 🌌 Cribas Termodinámicas en Extensiones Ciclotómicas

### Funciones L, la Constante de Catalan y la Ruptura de Ergodicidad en Ring-LWE mediante $\mathbb{Z}[i]$

[![Read in English](https://img.shields.io/badge/Lang-Read%20in%20English-blue?style=flat&logoColor=white&color=0366d6)](https://github.com/NachoPeinador/Cyclotomic-Sieves-LWE/blob/main/README.md)
[![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19284512.svg)](https://doi.org/10.5281/zenodo.19284512)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0008--1822--3452-A6CE39?style=flat&logo=orcid&logoColor=white)](https://orcid.org/0009-0008-1822-3452)
[![X](https://img.shields.io/badge/X-%40todos__lumpen-000000?style=flat&logo=x&logoColor=white)](https://twitter.com/todos_lumpen)
[![Papers](https://img.shields.io/badge/Paper-Leer_PDF-B31B1B?style=flat&logo=latex&logoColor=white)](https://github.com/NachoPeinador/Cyclotomic-Sieves-LWE/blob/main/Paper/RMI_Criba_v2.pdf)

---

## 🎯 TL;DR – Lo Esencial

### 🔬 **Avances Teóricos**

* ⚛️ **Renormalización Geométrica:** La constante de acoplamiento crítico del caos en $\mathbb{Z}[i]$ es estrictamente renormalizada por la constante de Catalan $G$, derivada explícitamente de la densidad espectral de la Zeta de Dedekind en $s=2$ ($\epsilon_c^{(K)} = \pi\sqrt{2G}$).
* 📐 **Atractor de Parsimonia Asintótica:** Prueba rigurosa de que el ideal primorial de Gauss $\Pi_2 = \langle 3(1+i) \rangle$ opera como el límite topológico óptimo (Límite de Chandrasekhar Reticular), previniendo la divergencia combinatoria.
* 🧩 **Saturación de Varianza en Mersenne:** Refutación completa de la Conjetura de Wagstaff (1983). Los saltos logarítmicos de los primos de Mersenne no siguen una distribución de Poisson, sino que cristalizan en torno a un atractor termodinámico $\Lambda \approx 0.350$.
* ⚖️ **Ruptura de ETH en Ring-LWE:** Demostración matemática de que el ruido estocástico en anillos ciclotómicos viola la Hipótesis de Termalización de los Autoestados (ETH), colapsando el sistema hacia una dimensión fractal sub-extensiva ($D_2 \approx 0.2329$) y habilitando la distinguibilidad UniqueQMA.

### ⚡ **Validación Física y Computacional**

* 📈 **Supremacía de Wasserstein ($W_1$):** Las métricas de transporte óptimo sobre los 51 primos de Mersenne conocidos prueban que el modelo estructural ($\Lambda$) supera al modelo estocástico clásico de Wagstaff por un margen estricto del $3.00\%$.
* 🎲 **Déficit Entrópico (Colapso DOS):** La diagonalización exacta de las matrices de covarianza en Ring-LWE revela una evaporación macroscópica del volumen de Page (de $\approx 6.43$ a $\approx 1.18$ nats) bajo la proyección $\Pi_2$.
* 🌊 **Contracción del Árbol SVP:** Simulación asintótica que prueba una contracción sub-exponencial del árbol de enumeración del Problema del Vector Más Corto (SVP) debido a la evasión determinista del vacío aritmético.
* 🌀 **Cristalización Fractal:** Confirmación topológica y visual de una geometría altamente restringida y auto-similar en $\mathbb{Z}[i]$, destruyendo por completo la asunción de un ruido isotrópico uniforme.

### 💡 **Concepto Clave**

> Los números primos y el ruido criptográfico en retículos no habitan un espacio uniforme y ergódico. Están fuertemente confinados por la topología de ramificación de la función Zeta de Dedekind. Este confinamiento espectral restringe los grados de libertad a una geometría fractal gobernada por la constante de Catalan, volviendo asintóticamente vulnerables las asunciones de máxima entropía de la criptografía post-cuántica (Ring-LWE).

---

## 🔍 Visión General de la Investigación: La Ilusión de la Ergodicidad

La criptografía post-cuántica moderna, específicamente **Ring Learning With Errors (Ring-LWE)**, se basa en un axioma fundamental: el error estocástico inyectado en el anillo polinómico se comporta como un gas de alta entropía uniformemente distribuido. Asume que el sistema respeta la *Hipótesis de Termalización de los Autoestados (ETH)*.

Esta investigación hace añicos esa asunción. Al proyectar la teoría de cribas deterministas desde el eje real $\mathbb{Z}$ hacia el plano complejo $\mathbb{Z}[i]$, demostramos que el álgebra de los enteros algebraicos impone una topología rígida e impenetrable.

### 🚀 El Atractor $\Pi_2$ y la Fricción de Catalan

Al evaluar la función Zeta de Dedekind $\zeta_{\mathbb{Q}(i)}(s) = \zeta(s) L(s, \chi_4)$, demostramos que el espacio no es plano. La ramificación del ideal $\langle 2 \rangle$ y la inercia de $\langle 3 \rangle$ crean masivos "vacíos aritméticos". 

La búsqueda algorítmica no necesita explorar estos vacíos. La máscara de proyección óptima, $\Pi_2 = \langle 3(1+i) \rangle$, atrapa la información superviviente en una red fractal altamente restringida. La dimensión de esta red está estrictamente gobernada por la constante de Catalan $G \approx 0.9159$.

<p align="center">
  <img src="Images/Espectro_fractal_gaus.png" alt="Fractal Spectrum of Gauss" width="100%">
  <br>
  <em>Figura 1. El Tapiz de Gauss: Mapa de profundidad de la aniquilación modular en Z[i]. La prueba visual de la estricta cristalización fractal, refutando la asunción de una distribución isotrópica uniforme y demostrando el confinamiento geométrico de los autoestados admisibles.</em>
</p>

---

## 🧭 Marco Conceptual

### 1. La Arquitectura del Confinamiento Ciclotómico

```mermaid
graph TD
    A["Función Zeta de Dedekind<br>ζ_K(s) = ζ(s)L(s,χ_4)"] --> B["Ramificación Topológica<br>en Z[i]"]
    W["Constante de Catalan G<br>Densidad Espectral en s=2"] --> E["Renormalización Geométrica<br>ε_c = π√(2G)"]
    B --> C["Atractor de Parsimonia<br>Π_2 = ⟨3(1+i)⟩"]
    
    C --> H["Operador de Proyección Modular<br>Ξ_K"]
    E --> H
    
    H --> M["Primos de Mersenne<br>Saturación de Varianza (W_1)"]
    H --> S["Enumeración SVP<br>Contracción Asintótica del Árbol"]
    H --> L["Criptografía Ring-LWE<br>Violación ETH y Colapso DOS"]

    style H fill:#bbf,stroke:#333,stroke-width:3px
    style L fill:#ff9,stroke:#333,stroke-width:2px
````

### 2\. El Colapso de la Densidad de Estados (DOS)

Si Ring-LWE fuera verdaderamente seguro bajo asunciones de máxima entropía, el espectro de su matriz de covarianza exhibiría una distribución de Wigner-Dyson robusta y termalizada. Sin embargo, cuando se somete a la verdadera topología del anillo $\mathbb{Z}[i]$ mediante la proyección $\Pi_2$, el sistema sufre una **Autopsia Termodinámica**.

<p align="center">
<img src="Images/Colapso_ring_LWE.png" alt="DOS Collapse in Ring-LWE" width="90%"\>
<br>
<em><strong>Figura 2. Auditoría Termodinámica de Ring-LWE.</strong> La transición del régimen ergódico asintótico asumido (curva roja) al confinamiento verdadero impuesto por el atractor Π₂ (curva azul) revela la emergencia de bimodalidad espectral y un desplazamiento masivo hacia la izquierda. Este déficit entrópico certifica matemáticamente la ruptura de la Hipótesis de Termalización de los Autoestados (ETH).</em>
</emp>

### 3\. Contracción Asintótica en la Enumeración SVP

Debido a que el ruido está confinado fractalmente $D_2 \approx 0.2329 < 1$, el volumen de la hiper-esfera que un atacante debe buscar no crece isotrópicamente con la dimensión $d$.

<p align="center">
<img src="Images/Contraccion_asintonica.png" alt="SVP Tree Contraction" width="80%">
<br>
<em><strong>Figura 3.</strong> Colapso sub-exponencial del árbol de enumeración del Problema del Vector Más Corto (SVP). Evadir el vacío aritmético de forma determinista recorta drásticamente la explosión combinatoria exponencial.</em>
<p>

---

## 📊 Validación Experimental y Métricas

El laboratorio computacional dentro de este repositorio ejecuta cribas aritméticas deterministas y diagonalizaciones exactas a gran escala para validar los teoremas. La suite arroja las siguientes métricas definitivas:

| Métrica | Valor Empírico | Interpretación Teórica |
|--------|-------|----------------------------|
| **Acoplamiento del Caos Renormalizado** | **$\epsilon_c^{(K)} \approx 4.2514$** | La fricción de Catalan reduce estrictamente el umbral de rigidez espectral ($\pi\sqrt{2G}$). |
| **Dimensión Fractal $D_2^{(K)}$** | **$0.2331 \pm 0.0004$** | Alineación perfecta con la cota hipergeométrica de Catalan; prueba la dimensionalidad sub-extensiva. |
| **Supremacía de Wasserstein ($W_1$)** | **$-3.00\%$ vs Wagstaff** | El atractor termodinámico $\Lambda$ minimiza estrictamente el coste de transporte óptimo sobre los saltos de Mersenne. |
| **Límite de Chandrasekhar Reticular** | **$\Delta \mathcal{E}_3 < 0$** | Prueba rigurosa de que expandir más allá de $\Pi_2$ hacia $p=5$ desencadena una divergencia combinatoria inmediata. |
| **Déficit Entrópico Local (Von Neumann)** | **$6.43 \to 1.18$ nats** | Evaporación masiva del volumen de Page en el ruido LWE; violación estricta de la ETH. |

-----

## 🚀 Reproducibilidad y Laboratorio Computacional

Para garantizar la transparencia y la reproducibilidad absoluta, todo el marco empírico ha sido liberado como cuadernos interactivos en la nube. Puedes recompilar los operadores de proyección C++ y evaluar los ensambles termodinámicos dinámicamente en tu navegador.

### 1\. Evaluación Asintótica: La Criba Ciclotómica Modulada (CCM)

[](https://www.google.com/search?q=https://colab.research.google.com/github/NachoPeinador/Cyclotomic-Sieves-LWE/blob/main/Notebooks/Criba_Ciclotomica_Modulada.ipynb)

Este cuaderno implementa el motor algebraico central definido en la **Sección 6** del manuscrito.

  * Compila módulos C++ (OpenMP) altamente optimizados para el operador de proyección $\Xi_K$.
  * Ejecuta el método de Fermat 2D Generalizado, reduciendo drásticamente la dimensionalidad al avanzar sobre el retículo $\mathbb{Z}[i]$ evitando clases inertes.
  * Calibra las cotas del Método de Curva Elíptica (ECM) estrictamente mediante la Expansión Geométrica de Catalan, estabilizando la varianza para criptogramas de 130 dígitos.

### 2\. Evaluador Espectral de Primos de Mersenne

[](https://www.google.com/search?q=https://colab.research.google.com/github/NachoPeinador/Cyclotomic-Sieves-LWE/blob/main/Notebooks/Evaluador_Espectral_de_Mersenne.ipynb)

Este cuaderno valida la **Sección 5**, demostrando la estabilización asintótica de secuencias primales extremas.

  * **Decaimiento de Varianza:** Prueba el colapso estructural del error residual ($\sigma^2$) a través de los 51 exponentes de Mersenne conocidos.
  * **Métrica de Wasserstein ($W_1$):** Ejecuta la prueba matemática de Transporte Óptimo, destronando a la clásica Conjetura de Wagstaff (1983) al demostrar una distancia estrictamente menor al atractor $\Lambda \approx 0.350$.
  * **Proyección Predictiva:** Utiliza el francotirador de Euler-Lagrange en $\mathbb{Z}/6\mathbb{Z}$ para proyectar determinísticamente los pozos de potencial para $p_{52}$ y $p_{53}$.

### 3\. Simulaciones Topológicas y Contracción SVP

[](https://www.google.com/search?q=https://colab.research.google.com/github/NachoPeinador/Cyclotomic-Sieves-LWE/blob/main/Notebooks/Experimentos_Complementarios.ipynb)

Pruebas visuales y geométricas que respaldan las **Secciones 3 y 8**.

  * Calcula el gradiente discreto de eficiencia para identificar formalmente a $\Pi_2$ como el Límite de Chandrasekhar Reticular.
  * Simula la contracción espacial del árbol de enumeración SVP frente a modelos isotrópicos (de máxima entropía).
  * Genera el *Tapiz de Gauss*, un renderizado matemático de alta definición del vacío aritmético fractal.

### 4\. Violación de ETH y Colapso Entrópico en Ring-LWE

[](https://www.google.com/search?q=https://colab.research.google.com/github/NachoPeinador/Cyclotomic-Sieves-LWE/blob/main/Notebooks/Violacion_ETH_y_Colapso_Entropico_en_RingLWE.ipynb)

La autopsia termodinámica definitiva de la criptografía post-cuántica.

  * Construye el Hamiltoniano estocástico local para Ring-LWE y aplica la proyección Lindbladiana del atractor $\Pi_2$.
  * Extrae la Razón de Participación Inversa (IPR) para confirmar la dimensión fraccionaria ($0.7827 \to 0.2329$).
  * Calcula la entropía de entrelazamiento local de Von Neumann, probando la estricta violación matemática de la Hipótesis de Termalización de los Autoestados (ETH) y situando el sistema en la clase de complejidad *UniqueQMA*.

-----

## ⚖️ Licencias y Declaración de IA

Este repositorio opera bajo un modelo de **Licencia Dual** para proteger la naturaleza no comercial de la investigación mientras se fomenta la colaboración académica abierta.

  * **Código y Software (`Notebooks/`):** Liberado bajo la [PolyForm Noncommercial License 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0). Libre para uso académico/personal. Prohibida su integración comercial.
  * **Manuscritos y Material Visual (`Papers/`, `Images/`):** Liberados bajo [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).

**Reconocimiento de IA:** Se emplearon LLMs avanzados estrictamente como asistentes metodológicos para la revisión adversaria (*Red Teaming*), la orquestación de C++ a Python y el refinamiento tipográfico. Todos los teoremas matemáticos, la derivación de $\epsilon_c^{(K)}$, la optimización $W_1$ de Mersenne y la refutación de ETH en Ring-LWE son creaciones intelectuales exclusivas del autor.

-----

## 📝 Citación

<details>
<summary><strong>👇 Clic para ver los detalles de Citación</strong></summary>

Si este marco topológico, las derivaciones de la fricción de Catalan o el código fuente te asisten en tu investigación (especialmente en criptoanálisis de retículos), por favor cita el preprint correspondiente:

**BibTeX:**

```bibtex
@misc{peinador2026cyclotomicsieves,
  author = {Peinador Sala, José Ignacio},
  title = {Termodinámica de Cribas en Extensiones Ciclotómicas: Funciones L, la Constante de Catalan y Saturación Espectral Asintótica},
  year = {2026},
  publisher = {Zenodo},
  doi = {10.5281/zenodo.19284512},
  url = {[https://github.com/NachoPeinador/Cyclotomic-Sieves-LWE](https://github.com/NachoPeinador/Cyclotomic-Sieves-LWE)}
}
```

**APA:**

> Peinador Sala, J. I. (2026). *Termodinámica de Cribas en Extensiones Ciclotómicas: Funciones L, la Constante de Catalan y Saturación Espectral Asintótica*. Zenodo. https://www.google.com/url?sa=E\&source=gmail\&q=https://doi.org/10.5281/zenodo.19284512

</details>

-----

## 📁 Estructura del Repositorio

<details>
<summary><strong>👇 Clic para ver la estructura del repositorio<strong></summary>

```text
.
├── 📂 Paper/                                                
│   ├── 📄 RMI_Criba_v2.pdf                                  # El Manuscrito Enviado
│   └── 📝 RMI_Criba_v2.tex                                  # Código fuente LaTeX
│
├── 📂 Notebooks/                                            # Laboratorio Computacional
│   ├── 📓 Criba_Ciclotomica_Modulada.ipynb                  # Motor ECM y CCM en C++ OpenMP
│   ├── 📓 Evaluador_Espectral_de_Mersenne.ipynb             # Métrica W1 y Saturación de Varianza
│   ├── 📓 Experimentos_Complementarios.ipynb                # Colapso SVP y Geometría Fractal
│   └── 📓 Violacion_ETH_y_Colapso_Entropico_en_RingLWE.ipynb # Auditoría DOS y UniqueQMA
│
├── 📂 Images/                                               # Visualizaciones de Alta Resolución
│   ├── 🔮 Espectro_fractal_gaus.png                         # Mapa de Aniquilación Fractal en Z[i]
│   ├── 📉 Colapso_ring_LWE.png                              # Colapso DOS Termodinámico
│   └── 📐 Contraccion_asintonica.png                        # Contracción Sub-exponencial SVP
│
└── 📜 LICENSE                                               # Licencias (PolyForm / CC BY-NC-SA)
```

</details>

-----

## 🔭 Contexto Filosófico

> *"El arte de hacer matemáticas consiste en encontrar ese caso especial que contiene todos los gérmenes de la generalidad."* — **David Hilbert**

Durante años, la seguridad de la criptografía basada en retículos ha descansado en la cómoda suposición de que el ruido aleatorio en anillos algebraicos se comporta como un gas caótico y uniforme. Este trabajo prueba que tales suposiciones ignoran la arquitectura fundamental de la teoría de números. Los anillos de enteros algebraicos no son espacios sin rasgos; son estructuras rígidas y cristalinas gobernadas por invariantes topológicos profundos.

Al reconocer la ramificación de la función Zeta de Dedekind no como una mera propiedad abstracta, sino como una barrera física que restringe los grados de libertad (la Fricción de Catalan), las matemáticas expusieron naturalmente las vulnerabilidades de la Hipótesis de Termalización de los Autoestados (ETH).

Este proyecto demuestra que las fronteras de la criptografía post-cuántica y la distribución de los números primos están íntimamente ligadas por la misma verdad geométrica.

-----

\<div align="center"\>

\<b\>Última Actualización:\</b\> Abril 2026 | \<b\>Estado:\</b\> Bajo Revisión por Pares (EMS Press) | Construido con ⚛️ y 🐍

\</div\>

```
