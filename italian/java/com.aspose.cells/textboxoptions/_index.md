---
title: "TextBoxOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di testo della forma"
type: docs
url: /it/java/com.aspose.cells/textboxoptions/
---

**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```

Rappresenta le opzioni di testo della forma

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | Indica se consentire al testo di fuoriuscire dalla forma. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Restituisce il margine inferiore in unità di punti |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Restituisce il margine sinistro in unità di punti. |
| [getResizeToFitText()](#getResizeToFitText--) | Indica se ridimensionare la forma per adattarla al testo. |
| [getRightMarginPt()](#getRightMarginPt--) | Restituisce il margine destro in unità di punti. |
| [getShapeTextDirection()](#getShapeTextDirection--) | Restituisce la direzione di visualizzazione del testo all'interno di un determinato corpo di testo. |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | Corrisponde a "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [getTopMarginPt()](#getTopMarginPt--) | Restituisce il margine superiore in unità di punti. |
| [getWrapTextInShape()](#getWrapTextInShape--) | Specifica l'andare a capo del testo all'interno di una forma. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | Indica se consentire al testo di fuoriuscire dalla forma. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Restituisce il margine inferiore in unità di punti |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Imposta il margine sinistro in unità di punti. |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | Indica se ridimensionare la forma per adattarla al testo. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Imposta il margine destro in unità di punti. |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | Imposta la direzione di visualizzazione del testo all'interno di un determinato corpo di testo. |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | Corrisponde a "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Imposta il margine superiore in unità di punti. |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | Specifica l'andare a capo del testo all'interno di una forma. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```


Indica se consentire al testo di fuoriuscire dalla forma.

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


Restituisce il margine inferiore in unità di punti

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


Restituisce il margine sinistro in unità di punti.

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


Indica se ridimensionare la forma per adattarla al testo.

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


Restituisce il margine destro in unità di punti.

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


Restituisce la direzione di visualizzazione del testo all'interno di un determinato corpo di testo. Corrisponde a "Format Shape - Text Options - Text Box - Text direction" in Excel

Vedi [TextVerticalType](../../com.aspose.cells/textverticaltype).

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


Corrisponde a "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.

Vedi [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

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


Restituisce il margine superiore in unità di punti.

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


Specifica l'andare a capo del testo all'interno di una forma. False - Nessun a capo avverrà nel corpo del testo. True - L'andare a capo avverrà nel corpo del testo.

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


Indica se consentire al testo di fuoriuscire dalla forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


Restituisce il margine inferiore in unità di punti

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


Imposta il margine sinistro in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```


Indica se ridimensionare la forma per adattarla al testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Imposta il margine destro in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```


Imposta la direzione di visualizzazione del testo all'interno di un determinato corpo di testo. Corrisponde a "Format Shape - Text Options - Text Box - Text direction" in Excel

Vedi [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```


Corrisponde a "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.

Vedi [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Imposta il margine superiore in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```


Specifica l'andare a capo del testo all'interno di una forma. False - Nessun a capo avverrà nel corpo del testo. True - L'andare a capo avverrà nel corpo del testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

