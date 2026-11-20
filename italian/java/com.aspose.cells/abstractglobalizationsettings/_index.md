---
title: "AbstractGlobalizationSettings"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le impostazioni di globalizzazione."
type: docs
url: /it/java/com.aspose.cells/abstractglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractGlobalizationSettings
```

Rappresenta le impostazioni di globalizzazione.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AbstractGlobalizationSettings()](#AbstractGlobalizationSettings--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Confronta due valori stringa secondo alcune regole di collazione. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Trasforma la stringa in un oggetto confrontabile secondo alcune regole di collazione. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractGlobalizationSettings() {#AbstractGlobalizationSettings--}
```
public AbstractGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Confronta due valori stringa secondo alcune regole di collazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| v1 | java.lang.String | la prima stringa |
| v2 | java.lang.String | la seconda stringa |
| ignoreCase | boolean | se ignorare la differenza tra maiuscole e minuscole durante il confronto dei valori |

**Returns:**
int - Intero che indica la relazione lessicale tra i due comparandi
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
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Trasforma la stringa in un oggetto confrontabile secondo alcune regole di collazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| v | java.lang.String | Il valore String deve essere confrontato con altri. |
| ignoreCase | boolean | se ignorare la differenza tra maiuscole e minuscole durante il confronto dei valori |

**Returns:**
java.lang.Comparable - L'oggetto può essere usato per confrontare o ordinare valori stringa
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

