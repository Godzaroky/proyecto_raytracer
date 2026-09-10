# Proyecto Raytracer

Raytracer por CPU escrito en Zig con raylib. Renderiza esferas con
iluminación difusa y especular (modelo de Phong) y sombras proyectadas.

## Requisitos

- Zig 0.16.0
- raylib-zig (se descarga con el gestor de paquetes de Zig)

## Compilar y ejecutar

```sh
zig build run
```

Para un render fluido conviene compilar optimizado:

```sh
zig build run -Doptimize=ReleaseFast
```

## Controles

| Tecla | Acción |
| ----- | ------ |
| `A` / `D` | Rotar la cámara horizontalmente |
| `W` / `S` | Rotar la cámara verticalmente |
| `ESC` | Salir |

## Estructura

| Archivo | Contenido |
| ------- | --------- |
| `src/main.zig` | Escena, bucle principal y trazado de rayos |
| `src/raytracer.zig` | Tipos base: `Material`, `Light`, `Intersect` |
| `src/sphere.zig` | Intersección rayo-esfera |
| `src/formas.zig` | Unión de tipos de figura |
| `src/camera.zig` | Cámara y `lookAt` |
| `src/framebuffer.zig` | Buffer de color y volcado a pantalla |
| `src/cute_colors.zig` | Colores en formato HTML en tiempo de compilación |

## Resultado

_Pendiente._
