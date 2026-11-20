---
title: "GridValidation"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le impostazioni di convalida dei dati."
type: docs
url: /it/java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

Rappresenta le impostazioni di convalida dei dati.
## Campi

| Campo | Descrizione |
| --- | --- |
| [ServerValidation](#ServerValidation) | Ottiene o imposta il nome della funzione JavaScript di convalida lato server. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | Aggiungi le impostazioni di convalida nella cella. |
| [addACell(String cellname)](#addACell-java.lang.String-) | Aggiungi le impostazioni di convalida nella cella. |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | Applica la validazione all'area. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | Rappresenta una raccolta di [GridCellArea](../../com.aspose.gridweb/gridcellarea) che contiene le impostazioni di convalida dei dati. |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | Ottiene il nome della funzione JavaScript di convalida lato client. |
| [getErrorMessage()](#getErrorMessage--) | Rappresenta il messaggio di errore della validazione dei dati. |
| [getErrorTitle()](#getErrorTitle--) | Rappresenta il titolo della finestra di dialogo di errore della validazione dei dati. |
| [getFormula1()](#getFormula1--) | Rappresenta il valore o l'espressione associata alla validazione dei dati. |
| [getFormula2()](#getFormula2--) | Rappresenta il valore o l'espressione associati alla seconda parte della convalida dei dati. |
| [getInputMessage()](#getInputMessage--) | Rappresenta il messaggio di errore della validazione dei dati. |
| [getInputTitle()](#getInputTitle--) | Rappresenta il titolo della finestra di dialogo di input della convalida dei dati. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Ottieni il valore per l'elenco della convalida per la cella specificata. |
| [getOperator()](#getOperator--) | Rappresenta l'operatore per la convalida dei dati. |
| [getRegEx()](#getRegEx--) | Ottiene la stringa dell'espressione regolare. |
| [getShowError()](#getShowError--) | Indica se il messaggio di errore della convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi. |
| [getShowInput()](#getShowInput--) | Indica se il messaggio di input della convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida. |
| [getValidationType()](#getValidationType--) | Ottiene il tipo di convalida. |
| [getValue1()](#getValue1--) | Rappresenta il valore associato alla convalida dei dati. |
| [getValueList()](#getValueList--) | Ottiene l'oggetto elenco valori. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | Ottiene se il valore della cella è obbligatorio. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Rimuovi le impostazioni di convalida nella cella. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | Rimuovi le impostazioni di convalida nell'intervallo. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | Imposta il nome della funzione JavaScript di convalida lato client. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Rappresenta il messaggio di errore della validazione dei dati. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Rappresenta il titolo della finestra di dialogo di errore della validazione dei dati. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Rappresenta il valore o l'espressione associata alla validazione dei dati. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Rappresenta il valore o l'espressione associati alla seconda parte della convalida dei dati. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Rappresenta il messaggio di errore della validazione dei dati. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Rappresenta il titolo della finestra di dialogo di input della convalida dei dati. |
| [setOperator(int value)](#setOperator-int-) | Rappresenta l'operatore per la convalida dei dati. |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | Imposta la stringa dell'espressione regolare. |
| [setRequired(boolean value)](#setRequired-boolean-) | Imposta se il valore della cella è obbligatorio. |
| [setShowError(boolean value)](#setShowError-boolean-) | Indica se il messaggio di errore della convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Indica se il messaggio di input della convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida. |
| [setValidationType(int value)](#setValidationType-int-) | Imposta il tipo di convalida. |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | Imposta l'oggetto elenco valori. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


Ottiene o imposta il nome della funzione JavaScript di convalida lato server.

**Remarks**

Utilizza la proprietà GridCustomServerValidation per specificare la convalida lato server.

### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```


Aggiungi le impostazioni di convalida nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```


Aggiungi le impostazioni di convalida nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellname | java.lang.String | nome della cella. |

### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```


Applica la validazione all'area.

**Remarks**

In questo metodo, rimuoveremo tutte le vecchie convalide in quest'area.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | L'area. |

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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```


Rappresenta una raccolta di [GridCellArea](../../com.aspose.gridweb/gridcellarea) che contiene le impostazioni di convalida dei dati.

**Remarks**

Le vecchie convalide sull'area non saranno rimosse se si aggiungono direttamente a questo elenco.

**Returns:**
java.util.ArrayList
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClientValidationFunction() {#getClientValidationFunction--}
```
public String getClientValidationFunction()
```


Ottiene il nome della funzione JavaScript di convalida lato client.

**Remarks**

Usa la proprietà ClientValidationFunction per specificare il nome della funzione di convalida client. La funzione dovrebbe essere dichiarata in questa forma:
function customValicationFunction(source, value)
Il parametro "source" è l'oggetto cella. Il parametro "value" è il valore stringa di una cella da verificare. La funzione dovrebbe restituire true se il valore è valido.

**Returns:**
java.lang.String
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
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Rappresenta il valore o l'espressione associati alla seconda parte della convalida dei dati.

**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Rappresenta il messaggio di errore della validazione dei dati.

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
java.lang.Object - Il valore per produrre l'elenco di questa convalida per la cella specificata. Se l'elenco fa riferimento a un intervallo, il valore restituito sarà un oggetto ReferredArea; altrimenti il valore restituito può essere null, object[] o un semplice oggetto.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Rappresenta l'operatore per la convalida dei dati.

Vedi [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


Ottiene la stringa dell'espressione regolare.

**Returns:**
java.lang.String
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
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


Ottiene il tipo di convalida.

Vedi [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```


Rappresenta il valore associato alla convalida dei dati.

**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```


Ottiene l'oggetto elenco valori.

**Returns:**
java.util.ArrayList<java.lang.String>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRequired() {#isRequired--}
```
public boolean isRequired()
```


Ottiene se il valore della cella è obbligatorio.

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

### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```


Rimuovi le impostazioni di convalida nell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | L'intervallo che contiene le impostazioni di convalida dei dati. |

### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```


Imposta il nome della funzione JavaScript di convalida lato client.

**Remarks**

Usa la proprietà ClientValidationFunction per specificare il nome della funzione di convalida client. La funzione dovrebbe essere dichiarata in questa forma:
function customValicationFunction(source, value)
Il parametro "source" è l'oggetto cella. Il parametro "value" è il valore stringa di una cella da verificare. La funzione dovrebbe restituire true se il valore è valido.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Rappresenta il valore o l'espressione associati alla seconda parte della convalida dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Rappresenta il messaggio di errore della validazione dei dati.

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

Vedi [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


Imposta la stringa dell'espressione regolare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


Imposta se il valore della cella è obbligatorio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


Imposta il tipo di convalida.

Vedi [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


Imposta l'oggetto elenco valori.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.ArrayList<java.lang.String> |  |

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

