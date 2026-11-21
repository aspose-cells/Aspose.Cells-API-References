---
title: "AbstractFormulaChangeMonitor"
second_title: "Aspose.Cells för Java API-referens"
description: "Övervaka så att användaren kan följa förändringen av formler under vissa operationer."
type: docs
url: /sv/java/com.aspose.cells/abstractformulachangemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractFormulaChangeMonitor
```

Övervaka så att användaren kan följa förändringen av formler under vissa operationer.

**Remarks**

Till exempel, när ett område med celler tas bort eller infogas, kan formler i andra celler ändras på grund av förskjutning av referenser. Observera att metoder i övervakaren kan anropas flera gånger för ett objekt som innehåller formeln.

**Example**

```
         class MyFormulaChangeMonitor extends AbstractFormulaChangeMonitor
         {
             private final WorksheetCollection mWorksheets;
             public MyFormulaChangeMonitor(WorksheetCollection worksheets)
             {
                 mWorksheets = worksheets;
             }
             public /*override*/ void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
             {
                 System.out.println("Cell " + mWorksheets.get(sheetIndex).getName() + "!"
                     + CellsHelper.cellIndexToName(rowIndex, columnIndex)
                     + "'s formula was changed while inserting rows.");
             }
         }
         Workbook wb = new Workbook("template.xlsx");
         InsertOptions options = new InsertOptions();
         options.setFormulaChangeMonitor(new MyFormulaChangeMonitor(wb.getWorksheets()));
         wb.getWorksheets().get(0).getCells().insertRows(0, 2, options);
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [AbstractFormulaChangeMonitor()](#AbstractFormulaChangeMonitor--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)](#onCellFormulaChanged-int-int-int-) | Händelsen som utlöses när formeln i en cell ändras. |
| [onFormatConditionFormulaChanged(FormatCondition fc)](#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-) | Händelsen som utlöses när formeln för FormatCondition ändras. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractFormulaChangeMonitor() {#AbstractFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex) {#onCellFormulaChanged-int-int-int-}
```
public void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```


Händelsen som utlöses när formeln i en cell ändras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Bladindex för den ändrade cellen |
| rowIndex | int | Radindex för den ändrade cellen |
| columnIndex | int | Kolumnindex för den ändrade cellen |

### onFormatConditionFormulaChanged(FormatCondition fc) {#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-}
```
public void onFormatConditionFormulaChanged(FormatCondition fc)
```


Händelsen som utlöses när formeln för FormatCondition ändras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fc | [FormatCondition](../../com.aspose.cells/formatcondition) | FormatCondition-objektet vars formel har ändrats |

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

