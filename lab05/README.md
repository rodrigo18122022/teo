# Super Mario Bros - Pharo/Smalltalk Implementation

Una implementación del clásico Super Mario Bros (1985) desarrollada en Pharo/Smalltalk como parte del Laboratorio 05 del curso de Tecnología de Objetos.

## Integrantes

- **Choquehuanca Zapana, Hernan Andy** - [GitHub](https://github.com/hz07s/teo/tree/main/lab05)
- **Nina Calizaya Rafael Diego**   - [GitHub](https://github.com/drn2512/teo/tree/main/lab05)
- **Portugal Portugal Eduardo Sebastian Stephan** - [GitHub](https://github.com/Eduardo-P/teo/tree/main/lab05)
- **Quispe Huaman Rodrigo Ferdinand** - [GitHub](https://github.com/rodrigo18122022/teo/tree/main/lab05)
- **Salas Aguilar Juan Victor**  - [GitHub](https://github.com/salasvictor22/TeoLab/tree/main/lab05)

## Descripción

Este proyecto es una recreación del icónico juego Super Mario Bros utilizando Pharo/Smalltalk, un lenguaje de programación orientado a objetos puro. El desarrollo explora conceptos fundamentales de POO como herencia, polimorfismo y manejo de eventos en tiempo real.

### Características Implementadas

- **Física de juego**: Gravedad, fricción, saltos parabólicos
- **Entidades interactivas**: 
  - Jugador (Mario) con controles de movimiento y salto
  - Enemigos (Goombas y Koopas) con IA básica de patrulla
  - Items coleccionables (monedas, power-ups)
  - Bloques interactivos y plataformas
- **Sistema de colisiones**: Detección AABB entre todas las entidades
- **Renderizado gráfico**: Sprites animados con Roassal3
- **Gestión de estados**: Vidas, puntuación, condiciones de victoria/derrota
- **Nivel side-scroller**: Cámara desplazable con diseño de nivel hardcodeado

## Instalación en Pharo

1. **Descargar Pharo**
   - Visita [https://pharo.org/](https://pharo.org/)
   - Descarga Pharo 9 o superior
   - Descomprime y ejecuta la máquina virtual

2. **Instalar el juego**
   
   Ejecuta el siguiente código en un Playground:
   
   ```smalltalk
   Metacello new
       baseline: 'Mario';
       repository: 'github://hz07s/Mario:main';
       load.
   ```

3. **Ejecutar el juego**
   
   ```smalltalk
   MaGame new run
   ```

## Controles

- **Flechas Izquierda/Derecha**: Movimiento
- **Flecha Arriba/Espacio**: Salto
- **Flecha Abajo**: Agacharse

## Arquitectura

El proyecto sigue una arquitectura orientada a objetos modular:

- **MaEntity**: Clase base para todas las entidades (posición, velocidad, sprites)
- **MaPlayer**: Controlador del jugador con física y manejo de input
- **MaEnemy**: Clase base para enemigos (Goombas, Koopas)
- **MaLevel**: Gestor del nivel (carga de entidades, colisiones, update loop)
- **MaGame**: Controlador principal (inicialización, canvas Roassal3, game loop)
- **MaSprite**: Sistema de animación de sprites
- **MaLoader**: Carga de assets PNG

## Capturas

![Navegador de Sistema Pharo](https://user-images.githubusercontent.com/10532890/78724964-7ea42600-78fc-11ea-9ddd-42057e69542c.png)

*Sistema de clases del proyecto Mario en el navegador de Pharo*

## Objetivos Cumplidos

-  Investigación sobre Pharo/Smalltalk y su historia
-  Implementación de juego completo con física 2D
-  Aplicación de POO pura (herencia, polimorfismo, encapsulación)
-  Uso de Roassal3 para renderizado gráfico
-  Sistema de colisiones y detección de eventos
-  Trabajo colaborativo con control de versiones (Git)

## Referencias

- [Pharo Official Website](https://pharo.org)
- [Pharo by Example](https://books.pharo.org/pharo-by-example/)
- [Roassal3 Documentation](https://github.com/ObjectProfile/Roassal3)
- Alan Kay et al. - *The Early History of Smalltalk*, ACM SIGPLAN (1993)

## Documentación Completa

Para ver el informe técnico completo del laboratorio, consulta el documento adjunto que incluye:
- Investigación detallada sobre Pharo/Smalltalk
- Proceso de compilación y ejecución
- Diagramas de clases y flujo del programa
- Análisis de ventajas/desventajas del lenguaje
- Resultados y conclusiones del desarrollo

---

**Curso**: Tecnología de Objetos - VI Semestre  
**Docente**: Corrales Delgado Carlo Jose Luis  
**Año Lectivo**: 2025-B  
**Fecha**: 11/10/2025
