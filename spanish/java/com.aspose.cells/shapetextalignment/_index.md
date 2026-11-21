---
title: "ShapeTextAlignment"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración de la alineación del texto de las formas"
type: docs
url: /es/java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

Representa la configuración de la alineación de texto de la forma;

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina si esta instancia tiene el mismo valor que otro objeto [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) especificado. |
| [getAutoSize()](#getAutoSize--) | Indica si el tamaño de la forma se ajusta automáticamente según su contenido. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Devuelve el margen inferior en unidades de Points. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Devuelve el margen izquierdo en unidades de Points. |
| [getNumberOfColumns()](#getNumberOfColumns--) | Obtiene el número de columnas de texto en el rectángulo delimitador. |
| [getRightMarginPt()](#getRightMarginPt--) | Devuelve el margen derecho en unidades de Points. |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | Indica si se rota el texto con la forma. |
| [getRotationAngle()](#getRotationAngle--) | Obtiene la rotación de la forma. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Obtiene el tipo de desbordamiento horizontal del texto del cuadro de texto. |
| [getTextShapeType()](#getTextShapeType--) | Obtiene el tipo de transformación del texto. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Obtiene el tipo de desbordamiento vertical del texto del cuadro de texto. |
| [getTextVerticalType()](#getTextVerticalType--) | Obtiene la dirección del texto. |
| [getTopMarginPt()](#getTopMarginPt--) | Devuelve el margen superior en unidades de Points. |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | Indica si el margen del marco de texto es automático. |
| [isLockedText()](#isLockedText--) | Indica si la forma está bloqueada cuando la hoja de cálculo está protegida. |
| [isTextWrapped()](#isTextWrapped--) | Obtiene el tipo de ajuste de texto de la forma que contiene texto. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | Indica si el margen del marco de texto es automático. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica si el tamaño de la forma se ajusta automáticamente según su contenido. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Devuelve el margen inferior en unidades de Points. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Devuelve el margen izquierdo en unidades de Points. |
| [setLockedText(boolean value)](#setLockedText-boolean-) | Indica si la forma está bloqueada cuando la hoja de cálculo está protegida. |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Establece el número de columnas de texto en el rectángulo delimitador. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Devuelve el margen derecho en unidades de Points. |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | Indica si se rota el texto con la forma. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Establece la rotación de la forma. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Establece el tipo de desbordamiento horizontal del texto del cuadro de texto. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Establece el tipo de transformación del texto. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Establece el tipo de desbordamiento vertical del texto del cuadro de texto. |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | Establece la dirección del texto. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Establece el tipo de ajuste de texto de la forma que contiene texto. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Devuelve el margen superior en unidades de Points. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina si esta instancia tiene el mismo valor que otro objeto [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) especificado.

**Example**

```
         //You have to make sure that the index value in this line of code exists
         ShapeTextAlignment obj = workbook.getWorksheets().get(0).getShapes().get(0).getTextBody().getTextAlignment();
         if (shapeTextAlignment.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) para comparar con esta instancia. |

**Returns:**
boolean - true si el valor del parámetro obj es el mismo que el valor de esta instancia; de lo contrario, false. Si obj es null, este método devuelve false.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


Indica si el tamaño de la forma se ajusta automáticamente según su contenido.

**Example**

```
         shapeTextAlignment.setAutoSize(false);
```

**Returns:**
boolean
### getBottomMarginPt() {#getBottomMarginPt--}
```
public double getBottomMarginPt()
```


Devuelve el margen inferior en unidades de Points.

**Example**

```
         shapeTextAlignment.setBottomMarginPt(2.0d);
```

**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLeftMarginPt() {#getLeftMarginPt--}
```
public double getLeftMarginPt()
```


Devuelve el margen izquierdo en unidades de Points.

**Example**

```
         shapeTextAlignment.setLeftMarginPt(2.0d);
```

**Returns:**
double
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Obtiene el número de columnas de texto en el rectángulo delimitador.

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Devuelve el margen derecho en unidades de Points.

**Example**

```
         shapeTextAlignment.setRightMarginPt(2.0d);
```

**Returns:**
double
### getRotateTextWithShape() {#getRotateTextWithShape--}
```
public boolean getRotateTextWithShape()
```


Indica si se rota el texto con la forma.

**Example**

```
         shapeTextAlignment.setRotateTextWithShape(true);
```

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Obtiene la rotación de la forma.

**Example**

```
         shapeTextAlignment.setRotationAngle(90);
```

**Returns:**
double
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


Obtiene el tipo de desbordamiento horizontal del texto del cuadro de texto.

Ver [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         shapeTextAlignment.setTextHorizontalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


Obtiene el tipo de transformación del texto.

Ver [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         //Usually do not modify this value unless you know exactly what the modification will result in
         shapeTextAlignment.setTextShapeType(AutoShapeType.TEXT_BOX);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


Obtiene el tipo de desbordamiento vertical del texto del cuadro de texto.

Ver [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         shapeTextAlignment.setTextVerticalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextVerticalType() {#getTextVerticalType--}
```
public int getTextVerticalType()
```


Obtiene la dirección del texto.

Ver [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Example**

```
         shapeTextAlignment.setTextVerticalType(com.aspose.cells.TextVerticalType.HORIZONTAL);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


Devuelve el margen superior en unidades de Points.

**Example**

```
         shapeTextAlignment.setTopMarginPt(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
### isAutoMargin() {#isAutoMargin--}
```
public boolean isAutoMargin()
```


Indica si el margen del marco de texto es automático.

**Example**

```
         shapeTextAlignment.setAutoMargin(true);
```

**Returns:**
boolean
### isLockedText() {#isLockedText--}
```
public boolean isLockedText()
```


Indica si la forma está bloqueada cuando la hoja de cálculo está protegida.

**Remarks**

Solo funciona cuando la hoja de cálculo está protegida.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Obtiene el tipo de ajuste de texto de la forma que contiene texto.

**Example**

```
         shapeTextAlignment.setTextWrapped(true);
```

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoMargin(boolean value) {#setAutoMargin-boolean-}
```
public void setAutoMargin(boolean value)
```


Indica si el margen del marco de texto es automático.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indica si el tamaño de la forma se ajusta automáticamente según su contenido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


Devuelve el margen inferior en unidades de Points.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


Devuelve el margen izquierdo en unidades de Points.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```


Indica si la forma está bloqueada cuando la hoja de cálculo está protegida.

**Remarks**

Solo funciona cuando la hoja de cálculo está protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Establece el número de columnas de texto en el rectángulo delimitador.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Devuelve el margen derecho en unidades de Points.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


Indica si se rota el texto con la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Establece la rotación de la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Establece el tipo de desbordamiento horizontal del texto del cuadro de texto.

Ver [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Establece el tipo de transformación del texto.

Ver [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Establece el tipo de desbordamiento vertical del texto del cuadro de texto.

Ver [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


Establece la dirección del texto.

Ver [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Establece el tipo de ajuste de texto de la forma que contiene texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Devuelve el margen superior en unidades de Points.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

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

