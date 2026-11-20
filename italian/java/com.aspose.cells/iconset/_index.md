---
title: "IconSet"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Descrive la regola di formattazione condizionale IconSet."
type: docs
url: /it/java/com.aspose.cells/iconset/
---

**Inheritance:**
java.lang.Object
```
public class IconSet
```

Descrivi la regola di formattazione condizionale IconSet. Questa regola di formattazione condizionale applica icone alle celle in base ai loro valori.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | Ottieni il[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) dalla collezione |
| [getCfvos()](#getCfvos--) | Ottieni l'istanza di CFValueObjects. |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | Restituisce il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone. |
| [getShowValue()](#getShowValue--) | Restituisce il flag che indica se mostrare i valori delle celle a cui è applicato questo set di icone. |
| [getType()](#getType--) | Restituisce il tipo di set di icone da visualizzare. |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | Indica se il set di icone è personalizzato. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | Imposta il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Imposta il flag che indica se mostrare i valori delle celle a cui è applicato questo set di icone. |
| [setType(int value)](#setType-int-) | Imposta il tipo di set di icone da visualizzare. |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```


Ottieni il[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) dalla collezione

**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```


Ottieni l'istanza di CFValueObjects.

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


Restituisce il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone. Il valore predefinito è false.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Restituisce il flag che indica se mostrare i valori delle celle a cui è applicato questo set di icone. Il valore predefinito è true.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Restituisce il tipo di set di icone da visualizzare. Impostare il tipo verificherà automaticamente se il conteggio corrente di Cfvos è conforme al nuovo tipo. Se non è conforme, i Cfvos vecchi saranno rimossi e verranno aggiunti i Cfvos predefiniti.

Vedi [IconSetType](../../com.aspose.cells/iconsettype).

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


Indica se il set di icone è personalizzato. Il valore predefinito è false.

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


Imposta il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Imposta il flag che indica se mostrare i valori delle celle a cui è applicato questo set di icone. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Imposta il tipo di set di icone da visualizzare. Impostare il tipo verificherà automaticamente se il conteggio corrente dei Cfvos è conforme al nuovo tipo. Se non è conforme, i vecchi Cfvos verranno rimossi e verranno aggiunti i Cfvos predefiniti.

Vedi [IconSetType](../../com.aspose.cells/iconsettype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

