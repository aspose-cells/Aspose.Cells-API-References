---
title: "AbstractFormulaChangeMonitor"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Monitor per l'utente per tenere traccia delle modifiche delle formule durante determinate operazioni."
type: docs
url: /it/java/com.aspose.cells/abstractformulachangemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractFormulaChangeMonitor
```

Monitor per l'utente per tenere traccia delle modifiche delle formule durante determinate operazioni.

**Remarks**

Ad esempio, durante l'eliminazione/inserimento di un intervallo di celle, le formule di altre celle possono essere modificate a causa dello spostamento dei riferimenti. Si prega di notare che i metodi nel monitor possono essere invocati più volte per un singolo oggetto che contiene la formula.

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
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AbstractFormulaChangeMonitor()](#AbstractFormulaChangeMonitor--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)](#onCellFormulaChanged-int-int-int-) | L'evento che verrà attivato quando la formula in una cella viene modificata. |
| [onFormatConditionFormulaChanged(FormatCondition fc)](#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-) | L'evento che verrà attivato quando la formula di FormatCondition viene modificata. |
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


L'evento che verrà attivato quando la formula in una cella viene modificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | L'indice del foglio della cella modificata |
| rowIndex | int | L'indice della riga della cella modificata |
| columnIndex | int | L'indice della colonna della cella modificata |

### onFormatConditionFormulaChanged(FormatCondition fc) {#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-}
```
public void onFormatConditionFormulaChanged(FormatCondition fc)
```


L'evento che verrà attivato quando la formula di FormatCondition viene modificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fc | [FormatCondition](../../com.aspose.cells/formatcondition) | L'oggetto FormatCondition la cui formula è stata modificata |

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

