---
title: "RenameStrategy"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Opzione di strategia per nomi duplicati di colonne."
type: docs
url: /it/java/com.aspose.cells/renamestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```

Opzione di strategia per nomi duplicati di colonne.

**Remarks**

Durante l'elaborazione dei dati con intestazioni, alcuni scenari richiedono che le intestazioni non siano duplicate per tutte le colonne. Ad esempio, quando si esportano dati in una datatable e l'intestazione deve essere presa come nome della colonna della datatable, i valori duplicati dell'intestazione sono invalidi. Per questo tipo di situazioni, l'utente può determinare come gestirle specificando questa strategia.
## Campi

| Campo | Descrizione |
| --- | --- |
| [DIGIT](#DIGIT) | Denominato con cifra. |
| [EXCEPTION](#EXCEPTION) | Genera un'eccezione. |
| [LETTER](#LETTER) | Denominato con lettera.. |
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
### DIGIT {#DIGIT}
```
public static final int DIGIT
```


Denominato con cifra. I nomi duplicati diventeranno ...1, ...2, ecc.

### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```


Genera un'eccezione.

### LETTER {#LETTER}
```
public static final int LETTER
```


Denominato con lettera.. I nomi duplicati diventeranno ...A, ...B, ecc.

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

