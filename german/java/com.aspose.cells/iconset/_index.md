---
title: "IconSet"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Beschreibt die IconSet-Bedingte-Formatierungsregel."
type: docs
url: /de/java/com.aspose.cells/iconset/
---

**Inheritance:**
java.lang.Object
```
public class IconSet
```

Beschreiben Sie die IconSet-Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel wendet Symbole auf Zellen basierend auf deren Werten an.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
 
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
 
         ca.StartRow = 0;
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.ICON_SET);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Icon Set
         IconSet iconSet = cond.getIconSet();
 
         //Set Icon Type
         iconSet.setType(IconSetType.ARROWS_3);
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | Rufen Sie das [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) aus der Sammlung ab. |
| [getCfvos()](#getCfvos--) | Rufen Sie die CFValueObjects-Instanz ab. |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | Gibt das Flag zurück, das angibt, ob die Standardreihenfolge der Symbole in diesem IconSet umgekehrt wird. |
| [getShowValue()](#getShowValue--) | Gibt das Flag zurück, das angibt, ob die Werte der Zellen angezeigt werden, auf die dieses IconSet angewendet wird. |
| [getType()](#getType--) | Gibt den anzuzeigenden IconSet-Typ zurück. |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | Gibt an, ob das IconSet benutzerdefiniert ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | Setzt das Flag, das angibt, ob die Standardreihenfolge der Symbole in diesem IconSet umgekehrt wird. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Setzt das Flag, das angibt, ob die Werte der Zellen angezeigt werden, auf die dieses IconSet angewendet wird. |
| [setType(int value)](#setType-int-) | Setzt den anzuzeigenden IconSet-Typ. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```


Rufen Sie das [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) aus der Sammlung ab.

**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```


Rufen Sie die CFValueObjects-Instanz ab.

**Returns:**
[ConditionalFormattingValueCollection](../../com.aspose.cells/conditionalformattingvaluecollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getReverse() {#getReverse--}
```
public boolean getReverse()
```


Gibt das Flag zurück, das angibt, ob die Standardreihenfolge der Symbole in diesem IconSet umgekehrt wird. Standardwert ist false.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Gibt das Flag zurück, das angibt, ob die Werte der Zellen angezeigt werden, auf die dieses IconSet angewendet wird. Standardwert ist true.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Gibt den anzuzeigenden IconSet-Typ zurück. Das Festlegen des Typs prüft automatisch, ob die aktuelle Anzahl der Cfvos mit dem neuen Typ übereinstimmt. Wenn nicht, werden alte Cfvos bereinigt und Standard‑Cfvos hinzugefügt.

Siehe [IconSetType](../../com.aspose.cells/iconsettype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCustom() {#isCustom--}
```
public boolean isCustom()
```


Gibt an, ob das Symbolset benutzerdefiniert ist. Standardwert ist false.

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




### setReverse(boolean value) {#setReverse-boolean-}
```
public void setReverse(boolean value)
```


Setzt das Flag, das angibt, ob die Standardreihenfolge der Symbole in diesem Symbolset umgekehrt wird. Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Setzt das Flag, das angibt, ob die Werte der Zellen, auf die dieses Symbolset angewendet wird, angezeigt werden sollen. Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Setzt den anzuzeigenden Symbolsettyp. Das Festlegen des Typs prüft automatisch, ob die aktuelle Anzahl der Cfvos mit dem neuen Typ übereinstimmt. Wenn nicht, werden alte Cfvos bereinigt und Standard‑Cfvos hinzugefügt.

Siehe [IconSetType](../../com.aspose.cells/iconsettype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

