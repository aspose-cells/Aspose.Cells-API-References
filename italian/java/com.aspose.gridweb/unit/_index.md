---
title: "Unit"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una misura di lunghezza"
type: docs
url: /it/java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

Rappresenta una misura di lunghezza
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Unit()](#Unit--) | il costruttore predefinito |
| [Unit(double value, int type)](#Unit-double-int-) | Inizializza una nuova istanza della struttura Unit con il numero a virgola mobile a doppia precisione specificato e UnitType. |
| [Unit(double value)](#Unit-double-) | Inizializza una nuova istanza della struttura Unit con il numero a virgola mobile a doppia precisione specificato. |
| [Unit(int value)](#Unit-int-) | Inizializza una nuova istanza della struttura Unit con l'intero con segno a 32 bit specificato. |
| [Unit(String value)](#Unit-java.lang.String-) | Inizializza una nuova istanza della struttura Unit con la lunghezza specificata. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | ottieni la stringa per il tipo, può restituire "px" "pt" "%" e così via; |
| [Parse(String s)](#Parse-java.lang.String-) | Converte la stringa specificata in un'Unit. |
| [Percentage(double n)](#Percentage-double-) | Crea un'Unit di tipo Percentage dal numero a virgola mobile a doppia precisione specificato. |
| [Pixel(int n)](#Pixel-int-) | Crea un'Unit di tipo Pixel dall'intero con segno a 32 bit specificato. |
| [Point(int n)](#Point-int-) | Crea un'Unit di tipo Point dall'intero con segno a 32 bit specificato. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Restituisce il tipo di unità dell'Unit. |
| [getValue()](#getValue--) | Restituisce la lunghezza dell'Unit. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | Restituisce un valore che indica se l'Unit è vuoto. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | ottieni la rappresentazione stringa dell'unità. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


il costruttore predefinito

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


Inizializza una nuova istanza della struttura Unit con il numero a virgola mobile a doppia precisione specificato e UnitType.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |
| tipo | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


Inizializza una nuova istanza della struttura Unit con il numero a virgola mobile a doppia precisione specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


Inizializza una nuova istanza della struttura Unit con l'intero con segno a 32 bit specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


Inizializza una nuova istanza della struttura Unit con la lunghezza specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


ottieni la stringa per il tipo, può restituire "px" "pt" "%" e così via;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tipo | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


Converte la stringa specificata in un'Unit.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


Crea un'Unit di tipo Percentage dal numero a virgola mobile a doppia precisione specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


Crea un'Unit di tipo Pixel dall'intero con segno a 32 bit specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


Crea un'Unit di tipo Point dall'intero con segno a 32 bit specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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
### getType() {#getType--}
```
public int getType()
```


Restituisce il tipo di unità dell'Unit.

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


Restituisce la lunghezza dell'Unit.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Restituisce un valore che indica se l'Unit è vuoto.

**Returns:**
boolean -
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


ottieni la rappresentazione stringa dell'unità.

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

