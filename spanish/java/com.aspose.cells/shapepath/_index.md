---
title: "ShapePath"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una ruta de creación compuesta por una serie de líneas y curvas de movimiento que, al combinarse, formarán una forma geométrica."
type: docs
url: /es/java/com.aspose.cells/shapepath/
---

**Inheritance:**
java.lang.Object
```
public class ShapePath
```

Representa una ruta de creación compuesta por una serie de movimientos, líneas y curvas que, al combinarse, formarán una forma geométrica.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ShapePath()](#ShapePath--) | Inicializa una nueva instancia de la clase [ShapePath](../../com.aspose.cells/shapepath). |
## Métodos

| Método | Descripción |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | Agrega un arco elíptico a la figura actual. |
| [close()](#close--) | Cierra la figura actual y comienza una nueva figura. |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | Agrega una curva cúbica B\u8305zier a la figura actual. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | Obtiene la altura de esta ruta en unidades de píxeles. |
| [getPathSegementList()](#getPathSegementList--) | Obtiene la lista [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getPathSegments()](#getPathSegments--) | Obtiene la lista [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getWidthPixel()](#getWidthPixel--) | Obtiene el ancho de esta ruta en unidades de píxeles. |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | Agrega un segmento de línea a la figura actual. |
| [moveTo(float x, float y)](#moveTo-float-float-) | Inicia una nueva figura desde el punto especificado sin cerrar la figura actual. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Obtiene la altura de esta ruta en unidades de píxeles. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Obtiene el ancho de esta ruta en unidades de píxeles. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```


Inicializa una nueva instancia de la clase [ShapePath](../../com.aspose.cells/shapepath).

### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```


Añade un arco elíptico a la figura actual. El punto de inicio es el punto final de la figura actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| wR | float | El medio ancho del área rectangular de la elipse \\u9225\\u5b27\\u20ac\\u5aa1 que dibuja el arco (Unidad: Pixel). |
| hR | float | El medio alto del área rectangular de la elipse \\u9225\\u5b27\\u20ac\\u5aa1 que dibuja el arco (Unidad: Pixel). |
| stAng | float | El ángulo de inicio del arco, medido en grados en sentido horario desde el eje x (Unidad: Grado). Este ángulo especificará qué ángulo a lo largo del supuesto camino circular se utilizará como posición inicial para dibujar el arco. Este ángulo de inicio se bloqueará a la última posición conocida del lápiz en la ruta de la forma, garantizando así una ruta de forma continua. |
| swAng | float | El ángulo de oscilación para un arco. Este ángulo especificará cuán lejos, angularmente, a lo largo del supuesto camino circular se extenderá el arco. La extensión desde el ángulo de inicio siempre será en dirección horaria alrededor del supuesto círculo.(Unidad: Grado) |

### close() {#close--}
```
public void close()
```


Cierra la figura actual y comienza una nueva figura. Si la figura actual contiene una secuencia de líneas y curvas conectadas, el método cierra el bucle conectando una línea desde el punto final hasta el punto de inicio.

### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```


Añade una curva cúbica B\\u8305zier a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad: Pixel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ctrX1 | float | La coordenada x del primer punto de control de la curva (Unidad: Pixel). |
| ctrY1 | float | La coordenada y del primer punto de control de la curva (Unidad: Pixel). |
| ctrX2 | float | La coordenada x del segundo punto de control de la curva (Unidad: Pixel). |
| ctrY2 | float | La coordenada y del segundo punto de control de la curva (Unidad: Pixel). |
| endX | float | La coordenada x del punto final de la curva (Unidad: Pixel). |
| endY | float | La coordenada y del punto final de la curva (Unidad: Pixel). |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Obtiene la altura de esta ruta en unidades de píxeles.

**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```


Obtiene la lista [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ShapePath.PathSegments. Esta propiedad será eliminada 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getPathSegments() {#getPathSegments--}
```
public ShapeSegmentPathCollection getPathSegments()
```


Obtiene la lista [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Obtiene el ancho de esta ruta en unidades de píxeles.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### lineTo(float x, float y) {#lineTo-float-float-}
```
public void lineTo(float x, float y)
```


Añade un segmento de línea a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad: Pixel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| x | float | La coordenada x del punto final del segmento de línea (Unidad: píxel). |
| y | float | La coordenada y del punto final del segmento de línea (Unidad: píxel). |

### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```


Inicia una nueva figura desde el punto especificado sin cerrar la figura actual. Todos los puntos posteriores añadidos a la ruta se añaden a esta nueva figura. Unidad: píxel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| x | float | La coordenada x del punto de inicio de la figura (Unidad: píxel). |
| y | float | La coordenada y del punto de inicio de la figura (Unidad: píxel). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Obtiene la altura de esta ruta en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Obtiene el ancho de esta ruta en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

