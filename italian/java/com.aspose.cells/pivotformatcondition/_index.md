---
title: "PivotFormatCondition"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una condizione di formato PivotTable nella collezione PivotFormatCondition."
type: docs
url: /it/java/com.aspose.cells/pivotformatcondition/
---

**Inheritance:**
java.lang.Object
```
public class PivotFormatCondition
```

Rappresenta una condizione di formato PivotTable nella collezione PivotFormatCondition.

**Remarks**

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare la classe [PivotConditionalFormat](../../com.aspose.cells/pivotconditionalformat). Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addColumnAreaCondition(PivotField columnField)](#addColumnAreaCondition-com.aspose.cells.PivotField-) | Aggiunge il limite di formato condizionale PivotTable nei campi di colonna. |
| [addColumnAreaCondition(String fieldName)](#addColumnAreaCondition-java.lang.String-) | Aggiunge il limite di formato condizionale PivotTable nei campi di colonna. |
| [addDataAreaCondition(PivotField dataField)](#addDataAreaCondition-com.aspose.cells.PivotField-) | Aggiunge il limite di formato condizionale PivotTable nei campi di dati. |
| [addDataAreaCondition(String fieldName)](#addDataAreaCondition-java.lang.String-) | Aggiunge il limite di formato condizionale PivotTable nei campi di dati. |
| [addRowAreaCondition(PivotField rowField)](#addRowAreaCondition-com.aspose.cells.PivotField-) | Aggiunge il limite di formato condizionale PivotTable nei campi di riga. |
| [addRowAreaCondition(String fieldName)](#addRowAreaCondition-java.lang.String-) | Aggiunge il limite di formato condizionale PivotTable nei campi di riga. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Ottieni le condizioni per il formato condizionale della tabella pivot. |
| [getRuleType()](#getRuleType--) | Ottiene il tipo di regola per il formato condizionale della tabella pivot. |
| [getScopeType()](#getScopeType--) | Ottiene il tipo di ambito per il formato condizionale della tabella pivot. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setConditionalAreas()](#setConditionalAreas--) | Imposta le aree condizionali dell'oggetto PivotFormatCondition. |
| [setRuleType(int value)](#setRuleType-int-) | Imposta il tipo di regola per il formato condizionale della tabella pivot. |
| [setScopeType(int value)](#setScopeType-int-) | Imposta il tipo di ambito per il formato condizionale della tabella pivot. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColumnAreaCondition(PivotField columnField) {#addColumnAreaCondition-com.aspose.cells.PivotField-}
```
public void addColumnAreaCondition(PivotField columnField)
```


Aggiunge il limite di formato condizionale PivotTable nei campi di colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnField | [PivotField](../../com.aspose.cells/pivotfield) | Il PivotField nei campi di colonna. |

### addColumnAreaCondition(String fieldName) {#addColumnAreaCondition-java.lang.String-}
```
public void addColumnAreaCondition(String fieldName)
```


Aggiunge il limite di formato condizionale PivotTable nei campi di colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldName | java.lang.String | Il nome di PivotField. |

### addDataAreaCondition(PivotField dataField) {#addDataAreaCondition-com.aspose.cells.PivotField-}
```
public void addDataAreaCondition(PivotField dataField)
```


Aggiunge il limite di formato condizionale PivotTable nei campi di dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataField | [PivotField](../../com.aspose.cells/pivotfield) | Il PivotField nei campi di dati. |

### addDataAreaCondition(String fieldName) {#addDataAreaCondition-java.lang.String-}
```
public void addDataAreaCondition(String fieldName)
```


Aggiunge il limite di formato condizionale PivotTable nei campi di dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldName | java.lang.String | Il nome di PivotField. |

### addRowAreaCondition(PivotField rowField) {#addRowAreaCondition-com.aspose.cells.PivotField-}
```
public void addRowAreaCondition(PivotField rowField)
```


Aggiunge il limite di formato condizionale PivotTable nei campi di riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowField | [PivotField](../../com.aspose.cells/pivotfield) | Il PivotField nei campi di riga. |

### addRowAreaCondition(String fieldName) {#addRowAreaCondition-java.lang.String-}
```
public void addRowAreaCondition(String fieldName)
```


Aggiunge il limite di formato condizionale PivotTable nei campi di riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldName | java.lang.String | Il nome di PivotField. |

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
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Ottieni le condizioni per il formato condizionale della tabella pivot.

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Ottiene il tipo di regola per il formato condizionale della tabella pivot.

Vedi [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Ottiene il tipo di ambito per il formato condizionale della tabella pivot.

Vedi [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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




### setConditionalAreas() {#setConditionalAreas--}
```
public void setConditionalAreas()
```


Imposta le aree condizionali dell'oggetto PivotFormatCondition.

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Imposta il tipo di regola per il formato condizionale della tabella pivot.

Vedi [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Imposta il tipo di ambito per il formato condizionale della tabella pivot.

Vedi [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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

