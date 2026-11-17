---
title: "Clase ShapePath"
linktitle: "ShapePath"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase ShapePath. Encapsula el objeto que representa shapepath en Go."
type: docs
weight: 200
url: /es/go-cpp/shapepath/
---

## ShapePath class

Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.

```go

type ShapePath struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewShapePath](./newshapepath/) | Inicializa una nueva instancia de la clase ShapePath. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetPathSegments](./getpathsegments/) | Obtiene la lista ShapeSegmentPathCollection |
| [GetWidthPixel](./getwidthpixel/) | Obtiene el ancho de esta ruta en unidades de píxeles. |
| [SetWidthPixel](./setwidthpixel/) | Obtiene el ancho de esta ruta en unidades de píxeles. |
| [GetHeightPixel](./getheightpixel/) | Obtiene la altura de esta ruta en unidades de píxeles. |
| [SetHeightPixel](./setheightpixel/) | Obtiene la altura de esta ruta en unidades de píxeles. |
| [MoveTo](./moveto/) | Inicia una nueva figura desde el punto especificado sin cerrar la figura actual. Todos los puntos posteriores añadidos a la ruta se añaden a esta nueva figura. Unidad: Pixel. |
| [LineTo](./lineto/) | Añade un segmento de línea a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad: Pixel. |
| [CubicBezierTo](./cubicbezierto/) | Añade una curva Bézier cúbica a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad: Pixel. |
| [ArcTo](./arcto/) | Añade un arco elíptico a la figura actual. El punto de inicio es el punto final de la figura actual. |
| [Close](./close/) | Cierra la figura actual e inicia una nueva figura. Si la figura actual contiene una secuencia de líneas y curvas conectadas, el método cierra el bucle conectando una línea desde el punto final hasta el punto de inicio. |
