---
title: "BindColumn"
second_title: "Aspose.Cells for Java API-Referenz"
description: "BindColumn."
type: docs
url: /de/java/com.aspose.gridweb/bindcolumn/
---

**Inheritance:**
java.lang.Object
```
public class BindColumn
```

BindColumn.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [BindColumn()](#BindColumn--) | Standardkonstruktor. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeStyle()](#getAlternativeStyle--) | Liefert den alternativen Stil der Spalte. |
| [getCaption()](#getCaption--) | Die Beschriftung der Spalte. |
| [getClass()](#getClass--) |  |
| [getColumnHeaderStyle()](#getColumnHeaderStyle--) | Liefert den Stil der Spalte. |
| [getCommandName()](#getCommandName--) | Der Befehlsname der Spalte. |
| [getCommandText()](#getCommandText--) | Der angezeigte Befehls-Text der Spalte. |
| [getCustomFormat()](#getCustomFormat--) | Die benutzerdefinierte Formatzeichenfolge. |
| [getDataField()](#getDataField--) | Liefert die Zeichenfolge des Datenfeldnamens. |
| [getEnableSort()](#getEnableSort--) | Gibt an, ob der Benutzer die Spaltenüberschrift anklicken kann, um nach diesem Feld zu sortieren. |
| [getImageUrl()](#getImageUrl--) | Die Bild-URL des Befehls-Hyperlinks. |
| [getName()](#getName--) | Nur zur Entwurfszeit verwendet. |
| [getNumberType()](#getNumberType--) | Liefert den Zahlentyp der Spalte. |
| [getStyle()](#getStyle--) | Liefert den Stil der Spalte. |
| [getUseAlternativeStyle()](#getUseAlternativeStyle--) | Liefert, ob der alternative Stil für die Spalte verwendet werden soll. |
| [getValidation()](#getValidation--) | Liefert das Validierungsobjekt der Spalte. |
| [getWidth()](#getWidth--) | Liefert oder setzt die Breite der Spalte. Nur Pixel oder Punkt werden akzeptiert. |
| [hashCode()](#hashCode--) |  |
| [isAutoCreated()](#isAutoCreated--) | Gibt an, ob die Spalte automatisch erstellt wird. |
| [isReadOnly()](#isReadOnly--) | Gibt an, ob die Spalte schreibgeschützt ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlternativeStyle(GridTableItemStyle value)](#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-) | Setzt den alternativen Stil der Spalte. |
| [setAutoCreated(boolean value)](#setAutoCreated-boolean-) | Gibt an, ob die Spalte automatisch erstellt wird. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Die Beschriftung der Spalte. |
| [setColumnHeaderStyle(GridTableItemStyle value)](#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-) | Setzt den Stil der Spalte. |
| [setCommandName(String value)](#setCommandName-java.lang.String-) | Der Befehlsname der Spalte. |
| [setCommandText(String value)](#setCommandText-java.lang.String-) | Der angezeigte Befehls-Text der Spalte. |
| [setCustomFormat(String value)](#setCustomFormat-java.lang.String-) | Die benutzerdefinierte Formatzeichenfolge. |
| [setDataField(String value)](#setDataField-java.lang.String-) | Setzt den Namen des Datenfelds als Zeichenkette. |
| [setEnableSort(boolean value)](#setEnableSort-boolean-) | Gibt an, ob der Benutzer die Spaltenüberschrift anklicken kann, um nach diesem Feld zu sortieren. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Die Bild-URL des Befehls-Hyperlinks. |
| [setNumberType(int value)](#setNumberType-int-) | Setzt den Zahlentyp der Spalte. |
| [setReadOnly(boolean value)](#setReadOnly-boolean-) | Gibt an, ob die Spalte schreibgeschützt ist. |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Setzt den Stil der Spalte. |
| [setUseAlternativeStyle(boolean value)](#setUseAlternativeStyle-boolean-) | Legt fest, ob der alternative Stil für die Spalte verwendet wird. |
| [setValidation(GridValidation value)](#setValidation-com.aspose.gridweb.GridValidation-) | Setzt das Validierungsobjekt der Spalte. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Liefert oder setzt die Breite der Spalte. Nur Pixel oder Punkt werden akzeptiert. |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAlternativeStyle() {#getAlternativeStyle--}
```
public GridTableItemStyle getAlternativeStyle()
```


Liefert den alternativen Stil der Spalte.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCaption() {#getCaption--}
```
public String getCaption()
```


Die Beschriftung der Spalte.

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


Liefert den Stil der Spalte.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCommandName() {#getCommandName--}
```
public String getCommandName()
```


Der Befehlsname der Spalte. Ein CellCommand-Hyperlink wird in der gebundenen Zelle erstellt, wenn die Eigenschaft CommandName gesetzt ist.

**Returns:**
java.lang.String
### getCommandText() {#getCommandText--}
```
public String getCommandText()
```


Der anzuzeigende Befehls‑Text der Spalte. Wenn er auf null gesetzt wird, verwendet die Zelle den Feldwert als Befehls‑Text.

**Returns:**
java.lang.String
### getCustomFormat() {#getCustomFormat--}
```
public String getCustomFormat()
```


Die benutzerdefinierte Formatzeichenfolge.

**Returns:**
java.lang.String
### getDataField() {#getDataField--}
```
public String getDataField()
```


Liefert die Zeichenfolge des Datenfeldnamens.

**Returns:**
java.lang.String
### getEnableSort() {#getEnableSort--}
```
public boolean getEnableSort()
```


Gibt an, ob der Benutzer die Spaltenüberschrift anklicken kann, um nach diesem Feld zu sortieren.

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


Die Bild-URL des Befehls-Hyperlinks.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Nur zur Entwurfszeit verwendet.

**Returns:**
java.lang.String
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Liefert den Zahlentyp der Spalte.

Siehe [NumberType](../../com.aspose.gridweb/numbertype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Liefert den Stil der Spalte.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getUseAlternativeStyle() {#getUseAlternativeStyle--}
```
public boolean getUseAlternativeStyle()
```


Liefert, ob der alternative Stil für die Spalte verwendet werden soll.

**Returns:**
boolean
### getValidation() {#getValidation--}
```
public GridValidation getValidation()
```


Liefert das Validierungsobjekt der Spalte.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Liefert oder setzt die Breite der Spalte. Nur Pixel oder Punkt werden akzeptiert.

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


Gibt an, ob die Spalte automatisch erstellt wird. Wenn true, wird die Spalte gelöscht, wenn der Benutzer zur Entwurfszeit die Datenquelle ändert.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Gibt an, ob die Spalte schreibgeschützt ist.

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


Setzt den alternativen Stil der Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoCreated(boolean value) {#setAutoCreated-boolean-}
```
public void setAutoCreated(boolean value)
```


Gibt an, ob die Spalte automatisch erstellt wird. Wenn true, wird die Spalte gelöscht, wenn der Benutzer zur Entwurfszeit die Datenquelle ändert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Die Beschriftung der Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setColumnHeaderStyle(GridTableItemStyle value) {#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setColumnHeaderStyle(GridTableItemStyle value)
```


Setzt den Stil der Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setCommandName(String value) {#setCommandName-java.lang.String-}
```
public void setCommandName(String value)
```


Der Befehlsname der Spalte. Ein CellCommand-Hyperlink wird in der gebundenen Zelle erstellt, wenn die Eigenschaft CommandName gesetzt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCommandText(String value) {#setCommandText-java.lang.String-}
```
public void setCommandText(String value)
```


Der anzuzeigende Befehls‑Text der Spalte. Wenn er auf null gesetzt wird, verwendet die Zelle den Feldwert als Befehls‑Text.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCustomFormat(String value) {#setCustomFormat-java.lang.String-}
```
public void setCustomFormat(String value)
```


Die benutzerdefinierte Formatzeichenfolge.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDataField(String value) {#setDataField-java.lang.String-}
```
public void setDataField(String value)
```


Setzt den Namen des Datenfelds als Zeichenkette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setEnableSort(boolean value) {#setEnableSort-boolean-}
```
public void setEnableSort(boolean value)
```


Gibt an, ob der Benutzer die Spaltenüberschrift anklicken kann, um nach diesem Feld zu sortieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


Die Bild-URL des Befehls-Hyperlinks.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Setzt den Zahlentyp der Spalte.

Siehe [NumberType](../../com.aspose.gridweb/numbertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setReadOnly(boolean value) {#setReadOnly-boolean-}
```
public void setReadOnly(boolean value)
```


Gibt an, ob die Spalte schreibgeschützt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Setzt den Stil der Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setUseAlternativeStyle(boolean value) {#setUseAlternativeStyle-boolean-}
```
public void setUseAlternativeStyle(boolean value)
```


Legt fest, ob der alternative Stil für die Spalte verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setValidation(GridValidation value) {#setValidation-com.aspose.gridweb.GridValidation-}
```
public void setValidation(GridValidation value)
```


Setzt das Validierungsobjekt der Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridValidation](../../com.aspose.gridweb/gridvalidation) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Liefert oder setzt die Breite der Spalte. Nur Pixel oder Punkt werden akzeptiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

