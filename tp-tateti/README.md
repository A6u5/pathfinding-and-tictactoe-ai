# Proyecto Tateti - Algoritmo Minimax

## 📋 Descripción

Este proyecto consiste en el desarrollo de una versión del juego Tateti (Tres en línea) que incorpora una inteligencia artificial basada en el algoritmo **Minimax**. Fue realizado como parte del trabajo práctico de la materia Programación III y permite enfrentar a un jugador humano contra la computadora, observar partidas entre dos inteligencias artificiales o jugar entre dos personas.

## 🎯 Objetivos

- Implementar el algoritmo Minimax.
- Aplicar teoría de juegos.
- Desarrollar una interfaz gráfica utilizando Pygame.
- Modelar el juego mediante estados y acciones.
- Evaluar decisiones óptimas en juegos de suma cero.

## 🤖 Algoritmo MiniMax
El algoritmo Minimax explora recursivamente todos los estados posibles del juego y selecciona la acción que maximiza la utilidad del jugador actual suponiendo que el adversario siempre realizará la mejor jugada posible. Dado que el espacio de estados del Tateti es reducido, la IA puede analizar el árbol completo de decisiones y garantizar un juego óptimo.

## 📁 Estructura del Proyecto

```
tp-tateti/
├── tateti.py           # Formulación del juego
├── estrategias.py      # Estrategias de juego
├── gui_pygame.py       # Interfaz gráfica moderna
├── main.py             # Punto de entrada de la aplicación
├── test.py             # Pruebas unitarias
├── requirements.txt    # Dependencias del proyecto
└── README.md           # Este archivo
```

## 🔧 Componentes

### 1. `tateti.py` - Formulación del juego ✅

Este módulo contiene la **formulación** del tateti según la teoría de juegos.

### 2. `estrategias.py` - Para implementar 🔨

**TODO**: Implementar el algoritmo Minimax en este módulo.

#### Funciones a completar:

```python
def estrategia_minimax(tateti: Tateti, estado: List[List[str]]) -> Tuple[int, int]:
    """
    Estrategia minimax: elige la mejor acción usando el algoritmo minimax.
    ....
    """
    # TODO: Implementar algoritmo minimax
```

### 3. `main.py` - Interfaz gráfica ✅

Aplicación completa con tres modos de juego:
- **Humano vs Humano**: Dos jugadores hacen click en las casillas
- **Humano vs Máquina**: El humano juega contra la IA
- **Máquina vs Máquina**: Observa dos IAs jugando

### 4. `test.py` - Pruebas ✅

Suite de pruebas para verificar tu implementación.

## 🚀 Instalación y Ejecución

### Requisitos del Sistema

- **Python 3.10+** (recomendado)
- **Sistema operativo**: Windows, macOS, o Linux

### 1. Instalar Dependencias

#### Opción A: Usando requirements.txt (Recomendado)
```bash
python3 -m pip install -r requirements.txt
```

#### Opción B: Instalación manual
```bash
python3 -m pip install pygame>=2.6.0
```

#### Verificar la instalación
```bash
python3 -c "import pygame; print('Pygame instalado correctamente:', pygame.version.ver)"
```

### 2. Ejecutar el Juego

```bash
python3 main.py
```

### 3. Ejecutar las Pruebas

```bash
python3 test.py
```

## 🔗 Bibliografía

- [Russell & Norvig - AI: A Modern Approach, Chapter 5](http://aima.cs.berkeley.edu/)
