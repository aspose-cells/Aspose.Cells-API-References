---
title: "GridValidationType"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il tipo di convalida dei dati."
type: docs
url: /it/java/com.aspose.gridweb/gridvalidationtype/
---

**Inheritance:**
java.lang.Object
```
public final class GridValidationType
```

Rappresenta il tipo di convalida dei dati.
## Campi

| Campo | Descrizione |
| --- | --- |
| [ANY_VALUE](#ANY-VALUE) | Tipo di convalida di qualsiasi valore. |
| [BOOLEAN](#BOOLEAN) | VERO o FALSO |
| [CHECK_BOX](#CHECK-BOX) | Visualizza la cella come una casella di controllo. |
| [CUSTOM](#CUSTOM) | Tipo di convalida personalizzata. |
| [CUSTOM_EXPRESSION](#CUSTOM-EXPRESSION) | Tipo di convalida personalizzata, usando espressione regolare. |
| [CUSTOM_FUNCTION](#CUSTOM-FUNCTION) | Convalida con funzione JavaScript personalizzata. |
| [CUSTOM_SERVER_FUNCTION](#CUSTOM-SERVER-FUNCTION) | Convalida con funzione lato server personalizzata. |
| [DATE](#DATE) | Tipo di convalida della data. |
| [DATE_TIME](#DATE-TIME) | DateTime (yyyy-MM-dd o yyyy-MM-dd hh:mm:ss). |
| [DECIMAL](#DECIMAL) | Tipo di convalida decimale. |
| [DROP_DOWN_LIST](#DROP-DOWN-LIST) | Mostra elenco a discesa. |
| [FREE_LIST](#FREE-LIST) | Tipo di convalida Lista libera. |
| [LIST](#LIST) | Tipo di convalida elenco. |
| [TEXT_LENGTH](#TEXT-LENGTH) | Tipo di convalida della lunghezza del testo. |
| [TIME](#TIME) | Tipo di convalida dell'ora. |
| [WHOLE_NUMBER](#WHOLE-NUMBER) | Tipo di convalida numero intero. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ANY_VALUE {#ANY-VALUE}
```
public static final int ANY_VALUE
```


Tipo di convalida di qualsiasi valore.

### BOOLEAN {#BOOLEAN}
```
public static final int BOOLEAN
```


VERO o FALSO

### CHECK_BOX {#CHECK-BOX}
```
public static final int CHECK_BOX
```


Visualizza la cella come una casella di controllo. E il valore della cella è True o False.

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Tipo di convalida personalizzata.

### CUSTOM_EXPRESSION {#CUSTOM-EXPRESSION}
```
public static final int CUSTOM_EXPRESSION
```


Tipo di convalida personalizzata, usando espressione regolare.

### CUSTOM_FUNCTION {#CUSTOM-FUNCTION}
```
public static final int CUSTOM_FUNCTION
```


Convalida con funzione JavaScript personalizzata.

**Remarks**

Usa la proprietà ClientValidationFunction per specificare il nome della funzione di convalida client. La funzione dovrebbe essere dichiarata in questa forma:
function customValicationFunction(source, value)
Il parametro "source" è l'oggetto cella. Il parametro "value" è il valore stringa di una cella da verificare. La funzione dovrebbe restituire true se il valore è valido.

### CUSTOM_SERVER_FUNCTION {#CUSTOM-SERVER-FUNCTION}
```
public static final int CUSTOM_SERVER_FUNCTION
```


Convalida con funzione lato server personalizzata.

**Remarks**

Usa la proprietà CustomServerFunction per specificare la convalida lato server. Di seguito il codice di esempio:
prima definisci la classe che implementa GridCustomServerValidation class myservervali : GridCustomServerValidation
...... poi aggiungi la convalida var gridValidationCollection = this.GridWeb.ActiveSheet.Validations;
GridValidation gv = gridValidationCollection.Add(new GridCellArea(1, 1, 2, 2));
gv.ValidationType = GridValidationType.CustomServerFunction; gv.ServerValidation = new myservervali(); poi imposta ClientValidationFunction per gestire la logica client quando la convalida server fallisce e restituisce il messaggio gv.ClientValidationFunction = "ValidationErrorClientFunction"; la funzione client deve essere dichiarata così: function ValidationErrorClientFunction(cell,msg) si prega di consultare la pagina demo per un riferimento dettagliato

### DATE {#DATE}
```
public static final int DATE
```


Tipo di convalida della data.

### DATE_TIME {#DATE-TIME}
```
public static final int DATE_TIME
```


DateTime (yyyy-MM-dd o yyyy-MM-dd hh:mm:ss).

### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Tipo di convalida decimale.

### DROP_DOWN_LIST {#DROP-DOWN-LIST}
```
public static final int DROP_DOWN_LIST
```


Mostra elenco a discesa.

### FREE_LIST {#FREE-LIST}
```
public static final int FREE_LIST
```


Tipo di convalida Lista libera.

### LIST {#LIST}
```
public static final int LIST
```


Tipo di convalida elenco.

### TEXT_LENGTH {#TEXT-LENGTH}
```
public static final int TEXT_LENGTH
```


Tipo di convalida della lunghezza del testo.

### TIME {#TIME}
```
public static final int TIME
```


Tipo di convalida dell'ora.

### WHOLE_NUMBER {#WHOLE-NUMBER}
```
public static final int WHOLE_NUMBER
```


Tipo di convalida numero intero.

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

