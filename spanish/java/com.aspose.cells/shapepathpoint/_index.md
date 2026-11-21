---
title: "ShapePathPoint"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica coordenadas de posición o marcadores de ángulo."
type: docs
url: /es/java/com.aspose.cells/shapepathpoint/
---

**Inheritance:**
java.lang.Object
```
public class ShapePathPoint
```

Especifique coordenadas de posición o marcadores de ángulo. Las coordenadas de posición representan las coordenadas de una ruta en un espacio de coordenadas (p. ej., X/Y). Los marcadores de ángulo indican cambios angulares en una ruta (p. ej., los ángulos de inicio y de arco).
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Especifica el tipo de valor del objeto actual. |
| [getX()](#getX--) | Obtiene la coordenada x para esta coordenada de posición. |
| [getXAngle()](#getXAngle--) | Cuando el objeto es un marcador de ángulo, obtenga o establezca el primer ángulo en grados. |
| [getXPixel()](#getXPixel--) | Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada x en píxeles. |
| [getY()](#getY--) | Obtiene la coordenada y para esta coordenada de posición. |
| [getYAngle()](#getYAngle--) | Cuando el objeto es un marcador de ángulo, obtenga o establezca el segundo ángulo en grados. |
| [getYPixel()](#getYPixel--) | Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada y en píxeles. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setX(int value)](#setX-int-) | Establece la coordenada x para esta coordenada de posición. |
| [setXAngle(int value)](#setXAngle-int-) | Cuando el objeto es un marcador de ángulo, obtenga o establezca el primer ángulo en grados. |
| [setXPixel(int value)](#setXPixel-int-) | Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada x en píxeles. |
| [setY(int value)](#setY-int-) | Obtiene la coordenada y para esta coordenada de posición. |
| [setYAngle(int value)](#setYAngle-int-) | Cuando el objeto es un marcador de ángulo, obtenga o establezca el segundo ángulo en grados. |
| [setYPixel(int value)](#setYPixel-int-) | Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada y en píxeles. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getType() {#getType--}
```
public int getType()
```


Especifica el tipo de valor del objeto actual.

Ver [ShapePathPointValueType](../../com.aspose.cells/shapepathpointvaluetype).

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Obtiene la coordenada x para esta coordenada de posición. Unidad EMUs.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use las propiedades ShapePathPoint.XPixel y ShapePathPoint.XAngle. Esta propiedad será eliminada 12 meses después a partir de agosto de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getXAngle() {#getXAngle--}
```
public int getXAngle()
```


Cuando el objeto es un marcador de ángulo, obtenga o establezca el primer ángulo en grados.

**Remarks**

Si este ángulo es el ángulo inicial de un arco. Este ángulo especificará qué ángulo a lo largo de la supuesta trayectoria circular se usará como posición inicial para dibujar el arco. Este ángulo inicial se bloqueará en la última posición conocida del lápiz en la ruta de forma. Así se garantiza una ruta de forma continua.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada x en píxeles.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Obtiene la coordenada y para esta coordenada de posición. Unidad EMUs.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use las propiedades ShapePathPoint.YPixel y ShapePathPoint.YAngle. Esta propiedad será eliminada 12 meses después a partir de agosto de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getYAngle() {#getYAngle--}
```
public int getYAngle()
```


Cuando el objeto es un marcador de ángulo, obtenga o establezca el segundo ángulo en grados.

**Remarks**

Si este ángulo es el ángulo de oscilación de un arco. Este ángulo especificará cuán lejos, en términos de ángulo, a lo largo de la supuesta trayectoria circular se extenderá el arco. La extensión desde el ángulo inicial siempre será en dirección horaria alrededor del círculo supuesto.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada y en píxeles.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Establece la coordenada x para esta coordenada de posición. Unidad EMUs.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use las propiedades ShapePathPoint.XPixel y ShapePathPoint.XAngle. Esta propiedad será eliminada 12 meses después a partir de agosto de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setXAngle(int value) {#setXAngle-int-}
```
public void setXAngle(int value)
```


Cuando el objeto es un marcador de ángulo, obtenga o establezca el primer ángulo en grados.

**Remarks**

Si este ángulo es el ángulo inicial de un arco. Este ángulo especificará qué ángulo a lo largo de la supuesta trayectoria circular se usará como posición inicial para dibujar el arco. Este ángulo inicial se bloqueará en la última posición conocida del lápiz en la ruta de forma. Así se garantiza una ruta de forma continua.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada x en píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Obtiene la coordenada y para esta coordenada de posición. Unidad EMUs.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use las propiedades ShapePathPoint.YPixel y ShapePathPoint.YAngle. Esta propiedad será eliminada 12 meses después a partir de agosto de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setYAngle(int value) {#setYAngle-int-}
```
public void setYAngle(int value)
```


Cuando el objeto es un marcador de ángulo, obtenga o establezca el segundo ángulo en grados.

**Remarks**

Si este ángulo es el ángulo de oscilación de un arco. Este ángulo especificará cuán lejos, en términos de ángulo, a lo largo de la supuesta trayectoria circular se extenderá el arco. La extensión desde el ángulo inicial siempre será en dirección horaria alrededor del círculo supuesto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada y en píxeles.

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

