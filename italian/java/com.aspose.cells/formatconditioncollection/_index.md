---
title: "FormatConditionCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la formattazione condizionale."
type: docs
url: /it/java/com.aspose.cells/formatconditioncollection/
---

**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```

Rappresenta la formattazione condizionale. Le FormatConditions possono contenere fino a tre formati condizionali.

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         //Saving the Excel file
         workbook.save("output.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | Aggiunge una condizione di formattazione e l'intervallo di celle interessato alle FormatConditions. Le FormatConditions possono contenere fino a tre formati condizionali. |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Aggiunge un intervallo di celle formattato condizionalmente. |
| [addCondition(int type)](#addCondition-int-) | Aggiungi una condizione di formattazione. |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | Aggiunge una condizione di formattazione. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene la condizione di formattazione per indice. |
| [getCellArea(int index)](#getCellArea-int-) | Ottiene l'intervallo di celle formattato condizionalmente per indice. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il conteggio delle condizioni. |
| [getRangeCount()](#getRangeCount--) | Ottiene il conteggio degli intervalli formattati condizionalmente. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | Rimuove l'intervallo di celle formattato condizionalmente per indice. |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | Rimuovi la formattazione condizionale nell'intervallo. |
| [removeCondition(int index)](#removeCondition-int-) | Rimuove la condizione di formattazione per indice. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```


Aggiunge una condizione di formattazione e l'intervallo di celle interessato a FormatConditions. FormatConditions può contenere fino a tre formati condizionali. I riferimenti ad altri fogli non sono consentiti nelle formule della formattazione condizionale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Intervallo di celle formattato condizionalmente. |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Tipo di formattazione condizionale. Può essere uno dei membri di FormatConditionType. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Operatore di confronto. Può essere uno dei membri di OperatorType. |
| formula1 | java.lang.String | Il valore o l'espressione associata alla formattazione condizionale. |
| formula2 | java.lang.String | Il valore o l'espressione associata alla formattazione condizionale |

**Returns:**
int[] - [0]: indice dell'oggetto condizione di formattazione; [1] indice dell'intervallo di celle interessato.
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```


Aggiunge un intervallo di celle formattato condizionalmente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Intervallo di celle formattato condizionalmente. |

**Returns:**
int - indice dell'intervallo di celle formattato condizionalmente.
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```


Aggiungi una condizione di formattazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Tipo di condizione di formattazione. |

**Returns:**
int - indice dell'oggetto condizione di formattazione;
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```


Aggiunge una condizione di formattazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Il tipo di condizione di formattazione. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Il tipo di operatore |
| formula1 | java.lang.String | Il valore o l'espressione associata alla formattazione condizionale. Se il valore di input inizia con '=', verrà interpretato come formula. Altrimenti verrà considerato come valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirli come formula nel formato: "=\\"=...\\"" |
| formula2 | java.lang.String | Il valore o l'espressione associata alla formattazione condizionale. Il formato di input è lo stesso di formula1 |

**Returns:**
int - indice dell'oggetto condizione di formattazione;
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
### get(int index) {#get-int-}
```
public FormatCondition get(int index)
```


Ottiene la condizione di formattazione per indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice della condizione di formattazione da restituire. |

**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```


Ottiene l'intervallo di celle formattato condizionalmente per indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice dell'intervallo di celle formattate condizionalmente. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Ottiene il conteggio delle condizioni.

**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Ottiene il conteggio degli intervalli formattati condizionalmente.

**Returns:**
int
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




### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```


Rimuove l'intervallo di celle formattato condizionalmente per indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice dell'intervallo di celle formattate condizionalmente da rimuovere. |

### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


Rimuovi la formattazione condizionale nell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | La startRow dell'intervallo. |
| startColumn | int | La startColumn dell'intervallo. |
| totalRows | int | Il numero di righe dell'intervallo. |
| totalColumns | int | Il numero di colonne dell'intervallo. |

**Returns:**
boolean - Restituisce TRUE, questa FormatCondtionCollection dovrebbe essere rimossa.
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```


Rimuove la condizione di formattazione per indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice della condizione di formattazione da rimuovere. |

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

