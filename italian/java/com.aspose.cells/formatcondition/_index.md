---
title: "FormatCondition"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la condizione della formattazione condizionale."
type: docs
url: /it/java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

Rappresenta la condizione della formattazione condizionale.

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
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | Ottieni l'istanza "AboveAverage" della formattazione condizionale. |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | Ottieni l'istanza "ColorScale" della formattazione condizionale. |
| [getDataBar()](#getDataBar--) | Ottieni l'istanza "DataBar" della formattazione condizionale. |
| [getFormula1()](#getFormula1--) | Ottiene il valore o l'espressione associati alla formattazione condizionale. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Ottiene il valore o l'espressione associati a questa condizione di formattazione. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Ottiene il valore o l'espressione della formattazione condizionale della cella. |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | Ottiene la formula della formattazione condizionale della cella. |
| [getFormula2()](#getFormula2--) | Ottiene il valore o l'espressione associati alla formattazione condizionale. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Ottiene il valore o l'espressione associati a questa condizione di formattazione. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Ottiene il valore o l'espressione della formattazione condizionale della cella. |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | Ottiene la formula della formattazione condizionale della cella. |
| [getIconSet()](#getIconSet--) | Ottieni l'istanza "IconSet" della formattazione condizionale. |
| [getOperator()](#getOperator--) | Ottiene il tipo di operatore della formattazione condizionale. |
| [getPriority()](#getPriority--) | La priorità di questa regola di formattazione condizionale. |
| [getStopIfTrue()](#getStopIfTrue--) | Vero, nessuna regola con priorità inferiore può essere applicata su questa regola, quando questa regola restituisce vero. |
| [getStyle()](#getStyle--) | Ottiene o imposta lo stile degli intervalli di celle formattate condizionalmente. |
| [getText()](#getText--) | Il valore di testo in una regola di formattazione condizionale \"text contains\". |
| [getTimePeriod()](#getTimePeriod--) | Il periodo di tempo applicabile in una regola di formattazione condizionale \"date occurrin\". |
| [getTop10()](#getTop10--) | Ottieni l'istanza \"Top10\" della formattazione condizionale. |
| [getType()](#getType--) | Ottiene se il tipo di formattazione condizionale. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Imposta il valore o l'espressione associata alla formattazione condizionale. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Imposta il valore o l'espressione associata a questa condizione di formattazione. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Imposta il valore o l'espressione associata alla formattazione condizionale. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Imposta il valore o l'espressione associata a questa condizione di formattazione. |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | Imposta il valore o l'espressione associata a questa condizione di formattazione. |
| [setOperator(int value)](#setOperator-int-) | Imposta il tipo di operatore della formattazione condizionale. |
| [setPriority(int value)](#setPriority-int-) | La priorità di questa regola di formattazione condizionale. |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | Vero, nessuna regola con priorità inferiore può essere applicata su questa regola, quando questa regola restituisce vero. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Ottiene o imposta lo stile degli intervalli di celle formattate condizionalmente. |
| [setText(String value)](#setText-java.lang.String-) | Il valore di testo in una regola di formattazione condizionale \"text contains\". |
| [setTimePeriod(int value)](#setTimePeriod-int-) | Il periodo di tempo applicabile in una regola di formattazione condizionale \"date occurrin\". |
| [setType(int value)](#setType-int-) | Imposta se il tipo di formattazione condizionale. |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


Ottieni l'istanza \"AboveAverage\" della formattazione condizionale. La regola dell'istanza predefinita evidenzia le celle che sono al di sopra della media per tutti i valori nell'intervallo. Valida solo per tipo = AboveAverage.

**Returns:**
[AboveAverage](../../com.aspose.cells/aboveaverage) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorScale() {#getColorScale--}
```
public ColorScale getColorScale()
```


Ottieni l'istanza \"ColorScale\" della formattazione condizionale. L'istanza predefinita è una \"green-yellow-red\" 3ColorScale. Valida solo per tipo = ColorScale.

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


Ottieni l'istanza \"DataBar\" della formattazione condizionale. Il colore dell'istanza predefinita è blu. Valida solo per tipo = DataBar.

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Ottiene il valore o l'espressione associati alla formattazione condizionale.

**Remarks**

Si prega di aggiungere tutte le aree prima di impostare la formula. Per impostare la formula per questa condizione, se il valore di input inizia con '=', verrà considerato una formula. Altrimenti verrà considerato un valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirli come formula nel formato: \"=\\\"=...\\\"\".

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Ottiene il valore o l'espressione associati a questa condizione di formattazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

**Returns:**
java.lang.String - Il valore o l'espressione associata a questa condizione di formattazione.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Ottiene il valore o l'espressione della formattazione condizionale della cella.

**Remarks**

La cella fornita deve essere contenuta da questa formattazione condizionale, altrimenti verrà restituito null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
java.lang.String - Il valore o l'espressione associata alla formattazione condizionale della cella.
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


Ottiene la formula della formattazione condizionale della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
java.lang.String - La formula.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Ottiene il valore o l'espressione associati alla formattazione condizionale.

**Remarks**

Si prega di aggiungere tutte le aree prima di impostare la formula. Per impostare la formula per questa condizione, se il valore di input inizia con '=', verrà considerato una formula. Altrimenti verrà considerato un valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirli come formula nel formato: \"=\\\"=...\\\"\".

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Ottiene il valore o l'espressione associati a questa condizione di formattazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

**Returns:**
java.lang.String - Il valore o l'espressione associata a questa condizione di formattazione.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Ottiene il valore o l'espressione della formattazione condizionale della cella.

**Remarks**

La cella fornita deve essere contenuta da questa formattazione condizionale, altrimenti verrà restituito null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
java.lang.String - Il valore o l'espressione associata alla formattazione condizionale della cella.
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


Ottiene la formula della formattazione condizionale della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
java.lang.String - La formula.
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


Ottieni l'istanza \"IconSet\" della formattazione condizionale. L'IconSetType dell'istanza predefinita è TrafficLights31. Valida solo per tipo = IconSet.

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


Ottiene il tipo di operatore della formattazione condizionale.

Vedi [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


La priorità di questa regola di formattazione condizionale. Questo valore è usato per determinare quale formato deve essere valutato e renderizzato. I valori numerici più bassi hanno priorità più alta rispetto a valori più alti, dove '1' è la priorità più alta.

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


Vero, nessuna regola con priorità inferiore può essere applicata su questa regola, quando questa regola restituisce vero. Si applica solo per Excel 2007;

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ottiene o imposta lo stile degli intervalli di celle formattate condizionalmente.

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


Il valore di testo in una regola di formattazione condizionale \"text contains\". Valida solo per tipo = containsText, notContainsText, beginsWith e endsWith. Il valore predefinito è null.

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


Il periodo di tempo applicabile in una regola di formattazione condizionale \"date occurrin\". Valida solo per tipo = timePeriod. Il valore predefinito è TimePeriodType.Today.

Vedi [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


Ottieni l'istanza \"Top10\" della formattazione condizionale. La regola dell'istanza predefinita evidenzia le celle i cui valori rientrano nella fascia Top10. Valida solo per tipo = Top10.

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


Ottiene se il tipo di formattazione condizionale.

Vedi [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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




### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Imposta il valore o l'espressione associata alla formattazione condizionale.

**Remarks**

Si prega di aggiungere tutte le aree prima di impostare la formula. Per impostare la formula per questa condizione, se il valore di input inizia con '=', verrà considerato una formula. Altrimenti verrà considerato un valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirli come formula nel formato: \"=\\\"=...\\\"\".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Imposta il valore o l'espressione associata a questa condizione di formattazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Il valore o l'espressione associata a questa condizione di formato. Se il valore di input inizia con '=', verrà considerato come formula. Altrimenti verrà considerato come valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirlo come formula nel formato: "=\\"=...\\"". |
| isR1C1 | boolean | Se la formula è una formula R1C1. |
| isLocal | boolean | Se la formula è formattata per la locale. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Imposta il valore o l'espressione associata alla formattazione condizionale.

**Remarks**

Si prega di aggiungere tutte le aree prima di impostare la formula. Per impostare la formula per questa condizione, se il valore di input inizia con '=', verrà considerato una formula. Altrimenti verrà considerato un valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirli come formula nel formato: \"=\\\"=...\\\"\".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Imposta il valore o l'espressione associata a questa condizione di formattazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Il valore o l'espressione associata a questa condizione di formato. Se il valore di input inizia con '=', verrà considerato come formula. Altrimenti verrà considerato come valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirlo come formula nel formato: "=\\"=...\\"". |
| isR1C1 | boolean | Se la formula è una formula R1C1. |
| isLocal | boolean | Se la formula è formattata per la locale. |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


Imposta il valore o l'espressione associata a questa condizione di formattazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula1 | java.lang.String | Il valore o l'espressione associata a questa condizione di formato. Se il valore di input inizia con '=', verrà considerato come formula. Altrimenti verrà considerato come valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirlo come formula nel formato: "=\\"=...\\"". |
| formula2 | java.lang.String | Il valore o l'espressione associata a questa condizione di formato. Il formato di input è lo stesso di formula1 |
| isR1C1 | boolean | Se la formula è una formula R1C1. |
| isLocal | boolean | Se la formula è formattata per la locale. |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Imposta il tipo di operatore della formattazione condizionale.

Vedi [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


La priorità di questa regola di formattazione condizionale. Questo valore è usato per determinare quale formato deve essere valutato e renderizzato. I valori numerici più bassi hanno priorità più alta rispetto a valori più alti, dove '1' è la priorità più alta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


Vero, nessuna regola con priorità inferiore può essere applicata su questa regola, quando questa regola restituisce vero. Si applica solo per Excel 2007;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Ottiene o imposta lo stile degli intervalli di celle formattate condizionalmente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Il valore di testo in una regola di formattazione condizionale \"text contains\". Valida solo per tipo = containsText, notContainsText, beginsWith e endsWith. Il valore predefinito è null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


Il periodo di tempo applicabile in una regola di formattazione condizionale \"date occurrin\". Valida solo per tipo = timePeriod. Il valore predefinito è TimePeriodType.Today.

Vedi [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Imposta se il tipo di formattazione condizionale.

Vedi [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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

