# algoritmica

Repositorio de la asignatura **Laboratorio de Programación** (E.E.S.T. N° 1 de Vicente López) correspondiente a la **Actividad 9: "Pensar antes de programar"**.

La consigna consiste en diseñar primero la solución en papel —mediante diagramas de flujo y pruebas de escritorio (matriz de ejecución)— y recién después trasladarla a código. Este repositorio reúne el informe académico, la captura de la matriz de ejecución y el programa en C++ que implementa los cuatro algoritmos planteados.

## Autor

**Alexander Luca Veit** ([@Xen-alt10](https://github.com/Xen-alt10)) · Curso 5°3 · Profesor: Mansilla Muñoz York E. · 17/11/2026

## Estructura del repositorio

```text
algoritmica/
├── capturas/
│   └── matriz_ejecucion.png      # Pruebas de escritorio de los 4 algoritmos
├── docs/
│   └── InformeEEST1_LPR2026_ACT09_AlexanderVeit_v1.0.0.pdf  # Informe (normas APA 7ª ed.)
├── src/
│   └── main.cpp                  # Implementación en C++ de los 4 algoritmos
├── .gitignore
├── LICENSE                       # Licencia MIT
└── README.md
```

## Algoritmos implementados

Todo el código se encuentra en [`src/main.cpp`](src/main.cpp) y se ejecuta en forma secuencial desde `main()`.

| # | Función | Descripción | Conceptos |
|---|---------|-------------|-----------|
| 1 | `sensorAprobacion()` | Lee dos notas, calcula el promedio e imprime `APROBADO` si es mayor o igual a 6, o `INTENSIFICACION` en caso contrario. | Variables `double`, constantes, `if/else` |
| 2 | `contadorVidas()` | Simula un contador de vidas que empieza en 3, muestra las vidas restantes en cada vuelta y finaliza con `GAME OVER`. | Bucle `while`, decremento |
| 3 | `registroJugador()` | Carga un `struct Jugador` (nickname, nivel y estado VIP) y da la bienvenida al servidor VIP o al servidor estándar según corresponda. | `struct`, `string`, `bool`, entrada de datos |
| 4 | `controlInventario()` | Recorre un arreglo de stock con 5 valores e informa las posiciones sin existencias. | Arreglos, `sizeof`, bucle `while`, `if` |

## Compilación y ejecución

El programa no tiene dependencias externas: alcanza con cualquier compilador de C++ (por ejemplo, GCC/MinGW en Windows o `g++` en Linux/macOS).

```bash
g++ -std=c++17 -o algoritmica src/main.cpp
```

En Windows con MinGW/PowerShell, el binario se genera con extensión `.exe`:

```powershell
g++ -std=c++17 -o algoritmica.exe src\main.cpp
.\algoritmica.exe
```

En Linux o macOS:

```bash
./algoritmica
```

> También se puede abrir `src/main.cpp` directamente en Visual Studio Code con la extensión de C/C++ y compilarlo usando la configuración de MinGW.

## Ejemplo de ejecución

```text
Ingrese nota1: 7
Ingrese nota2: 5
APROBADO
Jugador activo. Vidas restantes: 3
Jugador activo. Vidas restantes: 2
Jugador activo. Vidas restantes: 1
GAME OVER
Ingrese nickname: gise
Ingrese nivel: 3
Ingrese esVIP (1 = Verdadero, 0 = Falso): 1
Bienvenido al Servidor VIP, gise
ALERTA: Sin stock en pos. 1
ALERTA: Sin stock en pos. 4
```

## Matrices de ejecución

Las pruebas de escritorio de los cuatro diagramas se encuentran en [`capturas/matriz_ejecucion.png`](capturas/matriz_ejecucion.png).

## Informe

El Trabajo Práctico completo, con introducción, desarrollo, diagramas de flujo, pruebas de escritorio, conclusión y referencias según normas **APA 7ª edición**, está disponible en [`docs/InformeEEST1_LPR2026_ACT09_AlexanderVeit_v1.0.0.pdf`](docs/InformeEEST1_LPR2026_ACT09_AlexanderVeit_v1.0.0.pdf).

## Licencia

Distribuido bajo la licencia [MIT](LICENSE). Copyright (c) 2026 Xen-alt10.
