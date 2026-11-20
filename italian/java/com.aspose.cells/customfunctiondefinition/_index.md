---
title: "CustomFunctionDefinition"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Definizione della funzione personalizzata per il calcolo con il motore personalizzato dell'utente."
type: docs
url: /it/java/com.aspose.cells/customfunctiondefinition/
---

**Inheritance:**
java.lang.Object
```
public class CustomFunctionDefinition
```

Definizione della funzione personalizzata per il calcolo con il motore personalizzato dell'utente.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CustomFunctionDefinition()](#CustomFunctionDefinition--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArrayModeParameters(String functionName)](#getArrayModeParameters-java.lang.String-) | Restituisce gli indici dei parametri della funzione personalizzata fornita che devono essere calcolati in modalità array. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFunctionDefinition() {#CustomFunctionDefinition--}
```
public CustomFunctionDefinition()
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
### getArrayModeParameters(String functionName) {#getArrayModeParameters-java.lang.String-}
```
public int[] getArrayModeParameters(String functionName)
```


Restituisce gli indici dei parametri della funzione personalizzata fornita che devono essere calcolati in modalità array.

**Remarks**

Per un'espressione che deve essere calcolata, prendendo A:A+B:B come esempio: generalmente in modalità valore verrà calcolata a un singolo valore in base alla cella corrente. Ma in modalità array, tutti i valori di A1+B1, A2+B2, A3+B3, ... verranno calcolati e utilizzati per il calcolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionName | java.lang.String | Nome della funzione personalizzata. |

**Returns:**
int[] - Indici dei parametri che devono essere calcolati in modalità array per la funzione personalizzata fornita. Il valore predefinito è null, non esiste alcun parametro che debba essere calcolato in modalità array per la funzione personalizzata.
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

