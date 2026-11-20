---
title: "Colonna"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una singola colonna in un foglio di lavoro."
type: docs
url: /it/java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

Rappresenta una singola colonna in un foglio di lavoro.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Get first Column
         Column column = worksheet.getCells().getColumns().get(0);
 
         //Apply Style to first Column
         column.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applica formati a un'intera colonna. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | Ottiene il livello di gruppo della colonna. |
| [getIndex()](#getIndex--) | Ottiene l'indice di questa colonna. |
| [getStyle()](#getStyle--) | Ottiene lo stile di questa colonna. |
| [getWidth()](#getWidth--) | Ottiene la larghezza della colonna in unità di caratteri. |
| [hasCustomStyle()](#hasCustomStyle--) | Indica se questa colonna ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla cartella di lavoro). |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | se la colonna è compressa |
| [isHidden()](#isHidden--) | Indica se la colonna è nascosta. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | se la colonna è compressa |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Ottiene il livello di gruppo della colonna. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica se la colonna è nascosta. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Imposta lo stile di questa colonna. |
| [setWidth(double value)](#setWidth-double-) | Imposta la larghezza della colonna in unità di caratteri. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applica formati a un'intera colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'oggetto stile che verrà applicato. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flag che indicano le proprietà di formattazione applicate. |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Ottiene il livello di gruppo della colonna.

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ottiene l'indice di questa colonna.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ottiene lo stile di questa colonna.

**Remarks**

Modificare direttamente l'oggetto stile restituito non ha alcun effetto su questa colonna o su qualsiasi cella in questa colonna. È necessario chiamare il metodo [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) o [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) per applicare la modifica a questa colonna.

Lo stile della colonna è lo stile che verrà ereditato dalle celle in questa colonna (quelle celle che non hanno impostazioni di stile personalizzate, come le celle esistenti a cui non è stato impostato esplicitamente lo stile, o quelle che non sono state istanziate).

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


Ottiene la larghezza della colonna in unità di caratteri.

**Remarks**

Per i fogli di calcolo, la larghezza della colonna è misurata come il numero di caratteri della larghezza massima delle cifre dei numeri 0~9 così come renderizzati nel carattere dello stile normale.

**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indica se questa colonna ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla cartella di lavoro).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


se la colonna è compressa

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica se la colonna è nascosta.

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




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


se la colonna è compressa

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Ottiene il livello di gruppo della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica se la colonna è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Imposta lo stile di questa colonna.

**Remarks**

Questo metodo imposta solo lo stile fornito come stile predefinito per questa colonna, senza modificare le impostazioni di stile delle celle esistenti in questa colonna. Per aggiornare le impostazioni di stile delle celle esistenti allo stesso tempo con lo stile specificato, utilizzare [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | lo stile da utilizzare come stile predefinito per le celle in questa colonna. |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Imposta la larghezza della colonna in unità di caratteri.

**Remarks**

Per i fogli di calcolo, la larghezza della colonna è misurata come il numero di caratteri della larghezza massima delle cifre dei numeri 0~9 così come renderizzati nel carattere dello stile normale.

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

