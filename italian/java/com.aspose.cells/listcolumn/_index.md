---
title: "ListColumn"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una colonna in una Tabella."
type: docs
url: /it/java/com.aspose.cells/listcolumn/
---

**Inheritance:**
java.lang.Object
```
public class ListColumn
```

Rappresenta una colonna in una Tabella.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         ListColumn listColumn = table.getListColumns().get(4);
         listColumn.setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         listColumn.setFormula("=[A]");
         workbook.save("Book1.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | Ottiene la formula di questa colonna dell'elenco. |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | Ottiene la formula della riga dei totali di questa colonna dell'elenco. |
| [getDataStyle()](#getDataStyle--) | Ottiene lo stile dei dati in questa colonna della tabella. |
| [getFormula()](#getFormula--) | Ottiene la formula della colonna dell'elenco. |
| [getName()](#getName--) | Ottiene il nome della colonna. |
| [getRange()](#getRange--) | Ottiene l'intervallo di questa colonna dell'elenco. |
| [getTotalsCalculation()](#getTotalsCalculation--) | Ottiene il tipo di calcolo nella riga Totali della colonna dell'elenco. |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | Ottiene le etichette di visualizzazione della riga totale. |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | Indica se la formula è una formula matriciale. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | Imposta la formula per questa colonna dell'elenco. |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | Ottiene la formula della riga dei totali di questa colonna dell'elenco. |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | Imposta lo stile dei dati in questa colonna della tabella. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Imposta la formula della colonna dell'elenco. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome della colonna. |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | Imposta il tipo di calcolo nella riga Totali della colonna dell'elenco. |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | Imposta le etichette di visualizzazione della riga totale. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomCalculatedFormula(boolean isR1C1, boolean isLocal) {#getCustomCalculatedFormula-boolean-boolean-}
```
public String getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)
```


Ottiene la formula di questa colonna dell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

**Returns:**
java.lang.String - La formula di questa colonna dell'elenco.
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```


Ottiene la formula della riga dei totali di questa colonna dell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

**Returns:**
java.lang.String - La formula di questa colonna dell'elenco.
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```


Ottiene lo stile dei dati in questa colonna della tabella.

**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Ottiene la formula della colonna dell'elenco.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome della colonna.

**Remarks**

Se imposta il nome della colonna, anche il valore della cella corrispondente verrà modificato.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Ottiene l'intervallo di questa colonna dell'elenco.

**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```


Ottiene il tipo di calcolo nella riga Totali della colonna dell'elenco.

Vedi [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```


Ottiene le etichette di visualizzazione della riga totale.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Indica se la formula è una formula matriciale.

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




### setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomCalculatedFormula-java.lang.String-boolean-boolean-}
```
public void setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)
```


Imposta la formula per questa colonna dell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | la formula per questa colonna dell'elenco. |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```


Ottiene la formula della riga dei totali di questa colonna dell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | la formula per questa colonna dell'elenco. |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```


Imposta lo stile dei dati in questa colonna della tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Imposta la formula della colonna dell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome della colonna.

**Remarks**

Se imposta il nome della colonna, anche il valore della cella corrispondente verrà modificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```


Imposta il tipo di calcolo nella riga Totali della colonna dell'elenco.

Vedi [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```


Imposta le etichette di visualizzazione della riga totale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

