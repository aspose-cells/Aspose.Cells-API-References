---
title: "ShapeTextAlignment"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'impostazione dell'allineamento del testo delle forme"
type: docs
url: /it/java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

Rappresenta l'impostazione dell'allineamento del testo della forma;

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina se questa istanza ha lo stesso valore di un altro oggetto [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) specificato. |
| [getAutoSize()](#getAutoSize--) | Indica se la dimensione della forma è regolata automaticamente in base al suo contenuto. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Restituisce il margine inferiore in unità di punti |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Restituisce il margine sinistro in unità di punti |
| [getNumberOfColumns()](#getNumberOfColumns--) | Ottiene il numero di colonne di testo nel rettangolo di delimitazione. |
| [getRightMarginPt()](#getRightMarginPt--) | Restituisce il margine destro in unità di punti |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | Indica se il testo è ruotato con la forma. |
| [getRotationAngle()](#getRotationAngle--) | Ottiene la rotazione della forma. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Ottiene il tipo di overflow orizzontale del testo nella casella di testo. |
| [getTextShapeType()](#getTextShapeType--) | Ottiene il tipo di trasformazione del testo. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Ottiene il tipo di overflow verticale del testo nella casella di testo. |
| [getTextVerticalType()](#getTextVerticalType--) | Ottiene la direzione del testo. |
| [getTopMarginPt()](#getTopMarginPt--) | Restituisce il margine superiore in unità di punti |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | Indica se il margine del riquadro di testo è automatico. |
| [isLockedText()](#isLockedText--) | Indica se la forma è bloccata quando il foglio di lavoro è protetto. |
| [isTextWrapped()](#isTextWrapped--) | Ottiene il tipo di avvolgimento del testo della forma che contiene testo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | Indica se il margine del riquadro di testo è automatico. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica se la dimensione della forma è regolata automaticamente in base al suo contenuto. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Restituisce il margine inferiore in unità di punti |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Restituisce il margine sinistro in unità di punti |
| [setLockedText(boolean value)](#setLockedText-boolean-) | Indica se la forma è bloccata quando il foglio di lavoro è protetto. |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Imposta il numero di colonne di testo nel rettangolo di delimitazione. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Restituisce il margine destro in unità di punti |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | Indica se il testo è ruotato con la forma. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Imposta la rotazione della forma. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Imposta il tipo di overflow orizzontale del testo nella casella di testo. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Imposta il tipo di trasformazione del testo. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Imposta il tipo di overflow verticale del testo nella casella di testo. |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | Imposta la direzione del testo. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Imposta il tipo di avvolgimento del testo della forma che contiene testo. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Restituisce il margine superiore in unità di punti |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina se questa istanza ha lo stesso valore di un altro oggetto [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) specificato.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) da confrontare con questa istanza. |

**Returns:**
boolean - true se il valore del parametro obj è lo stesso del valore di questa istanza; altrimenti, false. Se obj è null, questo metodo restituisce false.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


Indica se la dimensione della forma è regolata automaticamente in base al suo contenuto.

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


Restituisce il margine inferiore in unità di punti

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


Restituisce il margine sinistro in unità di punti

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


Ottiene il numero di colonne di testo nel rettangolo di delimitazione.

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Restituisce il margine destro in unità di punti

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


Indica se il testo è ruotato con la forma.

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


Ottiene la rotazione della forma.

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


Ottiene il tipo di overflow orizzontale del testo nella casella di testo.

Vedi [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Ottiene il tipo di trasformazione del testo.

Vedi [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Ottiene il tipo di overflow verticale del testo nella casella di testo.

Vedi [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Ottiene la direzione del testo.

Vedi [TextVerticalType](../../com.aspose.cells/textverticaltype).

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


Restituisce il margine superiore in unità di punti

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


Indica se il margine del riquadro di testo è automatico.

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


Indica se la forma è bloccata quando il foglio di lavoro è protetto.

**Remarks**

Funziona solo quando il foglio di lavoro è protetto.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Ottiene il tipo di avvolgimento del testo della forma che contiene testo.

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


Indica se il margine del riquadro di testo è automatico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indica se la dimensione della forma è regolata automaticamente in base al suo contenuto.

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


Restituisce il margine sinistro in unità di punti

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```


Indica se la forma è bloccata quando il foglio di lavoro è protetto.

**Remarks**

Funziona solo quando il foglio di lavoro è protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Imposta il numero di colonne di testo nel rettangolo di delimitazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Restituisce il margine destro in unità di punti

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


Indica se il testo è ruotato con la forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Imposta la rotazione della forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Imposta il tipo di overflow orizzontale del testo nella casella di testo.

Vedi [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Imposta il tipo di trasformazione del testo.

Vedi [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Imposta il tipo di overflow verticale del testo nella casella di testo.

Vedi [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


Imposta la direzione del testo.

Vedi [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Imposta il tipo di avvolgimento del testo della forma che contiene testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Restituisce il margine superiore in unità di punti

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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

