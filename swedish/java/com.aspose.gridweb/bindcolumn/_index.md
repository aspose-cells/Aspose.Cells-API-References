---
title: "BindColumn"
second_title: "Aspose.Cells för Java API-referens"
description: "BindColumn."
type: docs
url: /sv/java/com.aspose.gridweb/bindcolumn/
---

**Inheritance:**
java.lang.Object
```
public class BindColumn
```

BindColumn.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [BindColumn()](#BindColumn--) | Standardkonstruktor. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeStyle()](#getAlternativeStyle--) | Hämtar den alternativa stilen för kolumnen. |
| [getCaption()](#getCaption--) | Rubriken för kolumnen. |
| [getClass()](#getClass--) |  |
| [getColumnHeaderStyle()](#getColumnHeaderStyle--) | Hämtar stilen för kolumnen. |
| [getCommandName()](#getCommandName--) | Kommandonamnet för kolumnen. |
| [getCommandText()](#getCommandText--) | Den visade kommandotexten för kolumnen. |
| [getCustomFormat()](#getCustomFormat--) | Den anpassade formatsträngen. |
| [getDataField()](#getDataField--) | Hämtar datafältets namnsträng. |
| [getEnableSort()](#getEnableSort--) | Anger om användaren kan klicka på kolumnrubriken för att sortera efter detta fält. |
| [getImageUrl()](#getImageUrl--) | Bild‑URL:en för kommandolänken. |
| [getName()](#getName--) | Endast för designtid. |
| [getNumberType()](#getNumberType--) | Hämtar taltypen för kolumnen. |
| [getStyle()](#getStyle--) | Hämtar stilen för kolumnen. |
| [getUseAlternativeStyle()](#getUseAlternativeStyle--) | Hämtar om den alternativa stilen ska användas för kolumnen. |
| [getValidation()](#getValidation--) | Hämtar valideringsobjektet för kolumnen. |
| [getWidth()](#getWidth--) | Hämtar eller sätter bredden på kolumnen. Endast pixlar eller punkter accepteras. |
| [hashCode()](#hashCode--) |  |
| [isAutoCreated()](#isAutoCreated--) | Anger om kolumnen skapas automatiskt. |
| [isReadOnly()](#isReadOnly--) | Anger om kolumnen är skrivskyddad. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlternativeStyle(GridTableItemStyle value)](#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-) | Ställer in den alternativa stilen för kolumnen. |
| [setAutoCreated(boolean value)](#setAutoCreated-boolean-) | Anger om kolumnen skapas automatiskt. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Rubriken för kolumnen. |
| [setColumnHeaderStyle(GridTableItemStyle value)](#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-) | Ställer in stilen för kolumnen. |
| [setCommandName(String value)](#setCommandName-java.lang.String-) | Kommandonamnet för kolumnen. |
| [setCommandText(String value)](#setCommandText-java.lang.String-) | Den visade kommandotexten för kolumnen. |
| [setCustomFormat(String value)](#setCustomFormat-java.lang.String-) | Den anpassade formatsträngen. |
| [setDataField(String value)](#setDataField-java.lang.String-) | Ställer in datafältets namnsträng. |
| [setEnableSort(boolean value)](#setEnableSort-boolean-) | Anger om användaren kan klicka på kolumnrubriken för att sortera efter detta fält. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Bild‑URL:en för kommandolänken. |
| [setNumberType(int value)](#setNumberType-int-) | Ställer in taltypen för kolumnen. |
| [setReadOnly(boolean value)](#setReadOnly-boolean-) | Anger om kolumnen är skrivskyddad. |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Ställer in stilen för kolumnen. |
| [setUseAlternativeStyle(boolean value)](#setUseAlternativeStyle-boolean-) | Ställer in om den alternativa stilen ska användas för kolumnen. |
| [setValidation(GridValidation value)](#setValidation-com.aspose.gridweb.GridValidation-) | Ställer in valideringsobjektet för kolumnen. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Hämtar eller sätter bredden på kolumnen. Endast pixlar eller punkter accepteras. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BindColumn() {#BindColumn--}
```
public BindColumn()
```


Standardkonstruktor.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAlternativeStyle() {#getAlternativeStyle--}
```
public GridTableItemStyle getAlternativeStyle()
```


Hämtar den alternativa stilen för kolumnen.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCaption() {#getCaption--}
```
public String getCaption()
```


Rubriken för kolumnen.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnHeaderStyle() {#getColumnHeaderStyle--}
```
public GridTableItemStyle getColumnHeaderStyle()
```


Hämtar stilen för kolumnen.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCommandName() {#getCommandName--}
```
public String getCommandName()
```


Kommandonamnet för kolumnen. En CellCommand Hyperlink kommer att skapas i den bundna cellen om egenskapen CommandName är inställd.

**Returns:**
java.lang.String
### getCommandText() {#getCommandText--}
```
public String getCommandText()
```


Den visade kommandotexten för kolumnen. Om den är satt till null kommer cellen att använda fältvärdet som kommandotext.

**Returns:**
java.lang.String
### getCustomFormat() {#getCustomFormat--}
```
public String getCustomFormat()
```


Den anpassade formatsträngen.

**Returns:**
java.lang.String
### getDataField() {#getDataField--}
```
public String getDataField()
```


Hämtar datafältets namnsträng.

**Returns:**
java.lang.String
### getEnableSort() {#getEnableSort--}
```
public boolean getEnableSort()
```


Anger om användaren kan klicka på kolumnrubriken för att sortera efter detta fält.

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


Bild‑URL:en för kommandolänken.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Endast för designtid.

**Returns:**
java.lang.String
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Hämtar taltypen för kolumnen.

Se [NumberType](../../com.aspose.gridweb/numbertype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Hämtar stilen för kolumnen.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getUseAlternativeStyle() {#getUseAlternativeStyle--}
```
public boolean getUseAlternativeStyle()
```


Hämtar om den alternativa stilen ska användas för kolumnen.

**Returns:**
boolean
### getValidation() {#getValidation--}
```
public GridValidation getValidation()
```


Hämtar valideringsobjektet för kolumnen.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Hämtar eller sätter bredden på kolumnen. Endast pixlar eller punkter accepteras.

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoCreated() {#isAutoCreated--}
```
public boolean isAutoCreated()
```


Anger om kolumnen skapas automatiskt. Om true kommer kolumnen att tas bort när användaren ändrar datakällan i designläget.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Anger om kolumnen är skrivskyddad.

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




### setAlternativeStyle(GridTableItemStyle value) {#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setAlternativeStyle(GridTableItemStyle value)
```


Ställer in den alternativa stilen för kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoCreated(boolean value) {#setAutoCreated-boolean-}
```
public void setAutoCreated(boolean value)
```


Anger om kolumnen skapas automatiskt. Om true kommer kolumnen att tas bort när användaren ändrar datakällan i designläget.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Rubriken för kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setColumnHeaderStyle(GridTableItemStyle value) {#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setColumnHeaderStyle(GridTableItemStyle value)
```


Ställer in stilen för kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setCommandName(String value) {#setCommandName-java.lang.String-}
```
public void setCommandName(String value)
```


Kommandonamnet för kolumnen. En CellCommand Hyperlink kommer att skapas i den bundna cellen om egenskapen CommandName är inställd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCommandText(String value) {#setCommandText-java.lang.String-}
```
public void setCommandText(String value)
```


Den visade kommandotexten för kolumnen. Om den är satt till null kommer cellen att använda fältvärdet som kommandotext.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCustomFormat(String value) {#setCustomFormat-java.lang.String-}
```
public void setCustomFormat(String value)
```


Den anpassade formatsträngen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDataField(String value) {#setDataField-java.lang.String-}
```
public void setDataField(String value)
```


Ställer in datafältets namnsträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setEnableSort(boolean value) {#setEnableSort-boolean-}
```
public void setEnableSort(boolean value)
```


Anger om användaren kan klicka på kolumnrubriken för att sortera efter detta fält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


Bild‑URL:en för kommandolänken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Ställer in taltypen för kolumnen.

Se [NumberType](../../com.aspose.gridweb/numbertype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setReadOnly(boolean value) {#setReadOnly-boolean-}
```
public void setReadOnly(boolean value)
```


Anger om kolumnen är skrivskyddad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Ställer in stilen för kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setUseAlternativeStyle(boolean value) {#setUseAlternativeStyle-boolean-}
```
public void setUseAlternativeStyle(boolean value)
```


Ställer in om den alternativa stilen ska användas för kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setValidation(GridValidation value) {#setValidation-com.aspose.gridweb.GridValidation-}
```
public void setValidation(GridValidation value)
```


Ställer in valideringsobjektet för kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridValidation](../../com.aspose.gridweb/gridvalidation) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Hämtar eller sätter bredden på kolumnen. Endast pixlar eller punkter accepteras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

