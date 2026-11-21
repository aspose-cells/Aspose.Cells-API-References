---
title: "TextBoxOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de texto de la forma"
type: docs
url: /es/java/com.aspose.cells/textboxoptions/
---

**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```

Representa las opciones de texto de la forma

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         int index = workbook.getWorksheets().get(0).getTextBoxes().add(0, 0, 350, 350);
         Shape shape = workbook.getWorksheets().get(0).getTextBoxes().get(index);
         shape.setText("This is test.");
 
         //do your business
 
         //Save the excel file.
         workbook.save("exmaple.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | Si permite que el texto desborde la forma. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Devuelve el margen inferior en unidades de Points. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Obtiene el margen izquierdo en unidades de puntos. |
| [getResizeToFitText()](#getResizeToFitText--) | Indica si se debe cambiar el tamaño de la forma para ajustarse al texto. |
| [getRightMarginPt()](#getRightMarginPt--) | Obtiene el margen derecho en unidades de puntos. |
| [getShapeTextDirection()](#getShapeTextDirection--) | Obtiene la dirección de visualización del texto dentro de un cuerpo de texto dado. |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Alineación vertical" en Excel. |
| [getTopMarginPt()](#getTopMarginPt--) | Obtiene el margen superior en unidades de puntos. |
| [getWrapTextInShape()](#getWrapTextInShape--) | Especifica el ajuste de texto dentro de una forma. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | Si permite que el texto desborde la forma. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Devuelve el margen inferior en unidades de Points. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Establece el margen izquierdo en unidades de puntos. |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | Indica si se debe cambiar el tamaño de la forma para ajustarse al texto. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Establece el margen derecho en unidades de puntos. |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | Establece la dirección de visualización del texto dentro de un cuerpo de texto dado. |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Alineación vertical" en Excel. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Establece el margen superior en unidades de puntos. |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | Especifica el ajuste de texto dentro de una forma. |
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
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```


Si permite que el texto desborde la forma.

**Example**

```
         shape.getTextBoxOptions().setAllowTextToOverflow(true);
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
         shape.getTextBoxOptions().setBottomMarginPt(0.2d);
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


Obtiene el margen izquierdo en unidades de puntos.

**Example**

```
         shape.getTextBoxOptions().setLeftMarginPt(0.2d);
```

**Returns:**
double
### getResizeToFitText() {#getResizeToFitText--}
```
public boolean getResizeToFitText()
```


Indica si se debe cambiar el tamaño de la forma para ajustarse al texto.

**Example**

```
         shape.getTextBoxOptions().setResizeToFitText(true);
```

**Returns:**
boolean
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Obtiene el margen derecho en unidades de puntos.

**Example**

```
         shape.getTextBoxOptions().setRightMarginPt(0.2d);
```

**Returns:**
double
### getShapeTextDirection() {#getShapeTextDirection--}
```
public int getShapeTextDirection()
```


Obtiene la dirección de visualización del texto dentro de un cuerpo de texto dado. Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Dirección del texto" en Excel

Ver [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Example**

```
         shape.getTextBoxOptions().setShapeTextDirection(TextVerticalType.VERTICAL);
```

**Returns:**
int
### getShapeTextVerticalAlignment() {#getShapeTextVerticalAlignment--}
```
public int getShapeTextVerticalAlignment()
```


Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Alineación vertical" en Excel.

Ver [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Example**

```
         shape.getTextBoxOptions().setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


Obtiene el margen superior en unidades de puntos.

**Example**

```
         shape.getTextBoxOptions().setTopMarginPt(0.2d);
```

**Returns:**
double
### getWrapTextInShape() {#getWrapTextInShape--}
```
public boolean getWrapTextInShape()
```


Especifica el ajuste de texto dentro de una forma. False - No se producirá ajuste en el cuerpo del texto. True - Se producirá ajuste en el cuerpo del texto.

**Example**

```
         shape.getTextBoxOptions().setWrapTextInShape(true);
```

**Returns:**
boolean
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




### setAllowTextToOverflow(boolean value) {#setAllowTextToOverflow-boolean-}
```
public void setAllowTextToOverflow(boolean value)
```


Si permite que el texto desborde la forma.

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


Establece el margen izquierdo en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```


Indica si se debe cambiar el tamaño de la forma para ajustarse al texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Establece el margen derecho en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```


Establece la dirección de visualización del texto dentro de un cuerpo de texto dado. Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Dirección del texto" en Excel

Ver [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```


Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Alineación vertical" en Excel.

Ver [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Establece el margen superior en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```


Especifica el ajuste de texto dentro de una forma. False - No se producirá ajuste en el cuerpo del texto. True - Se producirá ajuste en el cuerpo del texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

