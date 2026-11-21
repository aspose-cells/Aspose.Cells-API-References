---
title: "IconSet"
second_title: "Aspose.Cells för Java API-referens"
description: "Beskriv regeln för villkorsstyrd formatering med IconSet."
type: docs
url: /sv/java/com.aspose.cells/iconset/
---

**Inheritance:**
java.lang.Object
```
public class IconSet
```

Beskriv IconSet-regeln för villkorsstyrd formatering. Denna villkorsstyrda formateringsregel tillämpar ikoner på celler enligt deras värden.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | Hämta [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) från samlingen |
| [getCfvos()](#getCfvos--) | Hämta CFValueObjects-instansen. |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | Hämtar flaggan som indikerar om standardordningen för ikonerna i detta ikonset ska vändas. |
| [getShowValue()](#getShowValue--) | Hämtar flaggan som indikerar om värdena i de celler som detta ikonset tillämpas på ska visas. |
| [getType()](#getType--) | Hämtar ikonset-typen som ska visas. |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | Indikerar om ikonsetet är anpassat. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | Ställer in flaggan som indikerar om standardordningen för ikonerna i detta ikonset ska vändas. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Ställer in flaggan som indikerar om värdena i de celler som detta ikonset tillämpas på ska visas. |
| [setType(int value)](#setType-int-) | Ställer in ikonset-typen som ska visas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```


Hämta [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) från samlingen

**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```


Hämta CFValueObjects-instansen.

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


Hämtar flaggan som indikerar om standardordningen för ikonerna i detta ikonset ska vändas. Standardvärdet är falskt.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Hämtar flaggan som indikerar om värdena i de celler som detta ikonset tillämpas på ska visas. Standardvärdet är sant.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Hämtar ikonset-typen som ska visas. När typen ställs in kontrolleras automatiskt om antalet aktuella Cfvos överensstämmer med den nya typen. Om det inte överensstämmer kommer gamla Cfvos att rensas och standard-Cfvos att läggas till.

Se [IconSetType](../../com.aspose.cells/iconsettype).

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


Indikerar om ikonsetet är anpassat. Standardvärdet är falskt.

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


Ställer in flaggan som anger om standardordningen för ikonerna i den här ikonuppsättningen ska vändas. Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Ställer in flaggan som anger om värdena i cellerna som den här ikonuppsättningen tillämpas på ska visas. Standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Ställer in ikonuppsättningstypen som ska visas. När typen ställs in kontrolleras automatiskt om det aktuella antalet Cfvos överensstämmer med den nya typen. Om det inte överensstämmer rensas gamla Cfvos och standard-Cfvos läggs till.

Se [IconSetType](../../com.aspose.cells/iconsettype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

