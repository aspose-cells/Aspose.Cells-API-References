---
title: "Validazione"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le impostazioni di convalida dei dati."
type: docs
url: /it/java/com.aspose.cells/validation/
---

**Inheritance:**
java.lang.Object
```
public class Validation
```

Rappresenta le impostazioni di convalida dei dati.

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         	CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         	Validation validation = validations.get(validations.add(area));
         	validation.setType(com.aspose.cells.ValidationType.WHOLE_NUMBER);
         	validation.setOperator(OperatorType.BETWEEN);
         	validation.setFormula1("3");
         	validation.setFormula2("1234");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Applica la validazione all'area. |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | Applica la validazione all'area. |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | Applica la validazione alle aree specificate. |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | Copia la validazione. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | Rappresenta lo stile di avviso della validazione. |
| [getAreas()](#getAreas--) | Ottiene tutti i [CellArea](../../com.aspose.cells/cellarea) che contengono le impostazioni di validazione dei dati. |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | Rappresenta il messaggio di errore della validazione dei dati. |
| [getErrorTitle()](#getErrorTitle--) | Rappresenta il titolo della finestra di dialogo di errore della validazione dei dati. |
| [getFormula1()](#getFormula1--) | Rappresenta il valore o l'espressione associata alla validazione dei dati. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Ottiene il valore o l'espressione associata a questa validazione. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Ottiene il valore o l'espressione associata a questa validazione per una cella specifica. |
| [getFormula2()](#getFormula2--) | Rappresenta il valore o l'espressione associata alla validazione dei dati. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Ottiene il valore o l'espressione associata a questa validazione. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Ottiene il valore o l'espressione associata a questa validazione per una cella specifica. |
| [getIgnoreBlank()](#getIgnoreBlank--) | Indica se i valori vuoti sono consentiti dalla validazione dei dati dell'intervallo. |
| [getInCellDropDown()](#getInCellDropDown--) | Indica se la convalida dei dati visualizza un elenco a discesa che contiene valori accettabili. |
| [getInputMessage()](#getInputMessage--) | Rappresenta il messaggio di input della convalida dei dati. |
| [getInputTitle()](#getInputTitle--) | Rappresenta il titolo della finestra di dialogo di input della convalida dei dati. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Ottieni il valore per l'elenco della convalida per la cella specificata. |
| [getOperator()](#getOperator--) | Rappresenta l'operatore per la convalida dei dati. |
| [getShowError()](#getShowError--) | Indica se il messaggio di errore della convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi. |
| [getShowInput()](#getShowInput--) | Indica se il messaggio di input della convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida. |
| [getType()](#getType--) | Rappresenta il tipo di convalida dei dati. |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | Ottieni il valore della convalida sulla cella specifica. |
| [getValue1()](#getValue1--) | Rappresenta il primo valore associato alla convalida dei dati. |
| [getValue2()](#getValue2--) | Rappresenta il secondo valore associato alla convalida dei dati. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Rimuovi le impostazioni di convalida nella cella. |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | Rimuovi le impostazioni di convalida nell'intervallo. |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | Rimuove questa convalida dalle aree specificate. |
| [setAlertStyle(int value)](#setAlertStyle-int-) | Rappresenta lo stile di avviso della validazione. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Rappresenta il messaggio di errore della validazione dei dati. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Rappresenta il titolo della finestra di dialogo di errore della validazione dei dati. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Rappresenta il valore o l'espressione associata alla validazione dei dati. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Imposta il valore o l'espressione associata a questa convalida. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Rappresenta il valore o l'espressione associata alla validazione dei dati. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Imposta il valore o l'espressione associata a questa convalida. |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | Indica se i valori vuoti sono consentiti dalla validazione dei dati dell'intervallo. |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | Indica se la convalida dei dati visualizza un elenco a discesa che contiene valori accettabili. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Rappresenta il messaggio di input della convalida dei dati. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Rappresenta il titolo della finestra di dialogo di input della convalida dei dati. |
| [setOperator(int value)](#setOperator-int-) | Rappresenta l'operatore per la convalida dei dati. |
| [setShowError(boolean value)](#setShowError-boolean-) | Indica se il messaggio di errore della convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Indica se il messaggio di input della convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida. |
| [setType(int value)](#setType-int-) | Rappresenta il tipo di convalida dei dati. |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | Rappresenta il primo valore associato alla convalida dei dati. |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | Rappresenta il secondo valore associato alla convalida dei dati. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```


Applica la validazione all'area.

**Remarks**

È equivalente utilizzare [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\#addArea-CellArea-boolean-boolean-) con il controllo dell'intersezione e del bordo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | L'area. |

### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```


Applica la validazione all'area.

**Remarks**

In questo metodo, rimuoveremo tutte le vecchie convalide nell'area specificata. Per la prima (in alto a sinistra) delle aree applicate della Validation's, prima la sua StartRow è la più piccola, poi la sua StartColumn è la più piccola tra le aree che hanno la stessa StartRow minima.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | L'area. |
| checkIntersection | boolean | Indica se verificare l'intersezione dell'area specificata con le aree delle convalide esistenti. Se una convalida è stata applicata nell'area specificata (o in una sua parte), allora la convalida esistente dovrebbe essere rimossa prima dall'area specificata. Altrimenti potrebbero verificarsi corruzioni nelle Validations generate. Se l'utente è sicuro che l'area aggiunta non intersechi alcuna area esistente, questo parametro può essere impostato su false per ragioni di prestazioni. |
| checkEdge | boolean | Indica se verificare il bordo delle aree applicate di questa Validation's. Le impostazioni interne della Validation dipendono dalla prima (in alto a sinistra) delle sue aree applicate, quindi se l'area specificata diventerà la nuova prima (in alto a sinistra) delle aree applicate, le impostazioni interne dovrebbero essere modificate e ricostruite, altrimenti potrebbero verificarsi risultati inattesi. Se l'utente è sicuro che l'area aggiunta non sia la prima (in alto a sinistra), questo parametro può essere impostato su false per ragioni di prestazioni. |

### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```


Applica la validazione alle aree specificate.

**Remarks**

In questo metodo, rimuoveremo tutte le vecchie convalide nell'area specificata. Per la prima (in alto a sinistra) delle aree applicate della Validation's, prima la sua StartRow è la più piccola, poi la sua StartColumn è la più piccola tra le aree che hanno la stessa StartRow minima.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | Le aree. |
| checkIntersection | boolean | Indica se verificare l'intersezione dell'area specificata con le aree delle convalide esistenti. Se una convalida è stata applicata nell'area specificata (o in una sua parte), allora la convalida esistente dovrebbe essere rimossa prima dall'area specificata. Altrimenti potrebbero verificarsi corruzioni nelle Validations generate. Se l'utente è sicuro che tutte le aree aggiunte non intersechino alcuna area esistente, questo parametro può essere impostato su false per ragioni di prestazioni. |
| checkEdge | boolean | Indica se verificare il bordo delle aree applicate di questa Validation. Le impostazioni interne della Validation dipendono dalla prima (in alto a sinistra) delle sue aree applicate, quindi se una delle aree specificate diventerà la nuova prima (in alto a sinistra) delle aree applicate, le impostazioni interne dovrebbero essere modificate e ricostruite, altrimenti potrebbero verificarsi risultati inattesi. Se l'utente è sicuro che nessuna delle aree aggiunte sia la prima (in alto a sinistra), questo parametro può essere impostato su false per ragioni di prestazioni. |

### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```


Copia la validazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | La convalida della sorgente. |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | L'opzione di copia. |

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
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```


Rappresenta lo stile di avviso della validazione.

Vedi [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Ottiene tutti i [CellArea](../../com.aspose.cells/cellarea) che contengono le impostazioni di validazione dei dati.

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```


Rappresenta il messaggio di errore della validazione dei dati.

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


Rappresenta il titolo della finestra di dialogo di errore della validazione dei dati.

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Rappresenta il valore o l'espressione associata alla validazione dei dati.

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Ottiene il valore o l'espressione associata a questa validazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

**Returns:**
java.lang.String - Il valore o l'espressione associati a questa convalida.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Ottiene il valore o l'espressione associata a questa validazione per una cella specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
java.lang.String - Il valore o l'espressione associati a questa convalida.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Rappresenta il valore o l'espressione associata alla validazione dei dati.

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Ottiene il valore o l'espressione associata a questa validazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

**Returns:**
java.lang.String - Il valore o l'espressione associati a questa convalida.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Ottiene il valore o l'espressione associata a questa validazione per una cella specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
java.lang.String - Il valore o l'espressione associati a questa convalida.
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```


Indica se i valori vuoti sono consentiti dalla validazione dei dati dell'intervallo.

**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```


Indica se la convalida dei dati visualizza un elenco a discesa che contiene valori accettabili.

**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Rappresenta il messaggio di input della convalida dei dati.

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


Rappresenta il titolo della finestra di dialogo di input della convalida dei dati.

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


Ottieni il valore per l'elenco della convalida per la cella specificata.

**Remarks**

Solo per le convalide il cui tipo è List e che sono state applicate alla cella specificata, altrimenti verrà restituito null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
java.lang.Object - Il valore per produrre l'elenco di questa convalida per la cella specificata. Se l'elenco fa riferimento a un intervallo, il valore restituito sarà un oggetto [ReferredArea](../../com.aspose.cells/referredarea); altrimenti il valore restituito può essere null, object[] o un semplice oggetto.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Rappresenta l'operatore per la convalida dei dati.

Vedi [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


Indica se il messaggio di errore della convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi.

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


Indica se il messaggio di input della convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Rappresenta il tipo di convalida dei dati.

Vedi [ValidationType](../../com.aspose.cells/validationtype).

**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```


Ottieni il valore della convalida sulla cella specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |
| isValue1 | boolean | Indica se si sta ottenendo il primo valore. |

**Returns:**
java.lang.Object -
### getValue1() {#getValue1--}
```
public Object getValue1()
```


Rappresenta il primo valore associato alla convalida dei dati.

**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```


Rappresenta il secondo valore associato alla convalida dei dati.

**Returns:**
java.lang.Object
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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


Rimuovi le impostazioni di convalida nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```


Rimuovi le impostazioni di convalida nell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | le aree in cui queste impostazioni di convalida dovrebbero essere rimosse. |

### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```


Rimuove questa convalida dalle aree specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | le aree in cui queste impostazioni di convalida dovrebbero essere rimosse. |

### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```


Rappresenta lo stile di avviso della validazione.

Vedi [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


Rappresenta il messaggio di errore della validazione dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


Rappresenta il titolo della finestra di dialogo di errore della validazione dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Rappresenta il valore o l'espressione associata alla validazione dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Imposta il valore o l'espressione associata a questa convalida.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Il valore o l'espressione associati a questa condizione di formato. |
| isR1C1 | boolean | Se la formula è una formula R1C1. |
| isLocal | boolean | Se la formula è formattata per la locale. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Rappresenta il valore o l'espressione associata alla validazione dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Imposta il valore o l'espressione associata a questa convalida.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Il valore o l'espressione associati a questa condizione di formato. |
| isR1C1 | boolean | Se la formula è una formula R1C1. |
| isLocal | boolean | Se la formula è formattata per la locale. |

### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```


Indica se i valori vuoti sono consentiti dalla validazione dei dati dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```


Indica se la convalida dei dati visualizza un elenco a discesa che contiene valori accettabili.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Rappresenta il messaggio di input della convalida dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


Rappresenta il titolo della finestra di dialogo di input della convalida dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Rappresenta l'operatore per la convalida dei dati.

Vedi [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


Indica se il messaggio di errore della convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


Indica se il messaggio di input della convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Rappresenta il tipo di convalida dei dati.

Vedi [ValidationType](../../com.aspose.cells/validationtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```


Rappresenta il primo valore associato alla convalida dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```


Rappresenta il secondo valore associato alla convalida dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

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

