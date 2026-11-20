---
title: "ConditionalFormattingValue"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Descrive i valori dei punti di interpolazione in una barra dati a scala gradiente o in un set di icone."
type: docs
url: /it/java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

Descrive i valori dei punti di interpolazione in una scala gradiente, dataBar o iconSet.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Ottiene il tipo di questo oggetto valore di formattazione condizionale. |
| [getValue()](#getValue--) | Ottiene il valore di questo oggetto valore di formattazione condizionale. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | Ottiene il flag Maggiore o Uguale. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | Imposta il flag Maggiore o Uguale. |
| [setType(int value)](#setType-int-) | Imposta il tipo di questo oggetto valore di formattazione condizionale. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Imposta il valore di questo oggetto valore di formattazione condizionale. |
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
### getType() {#getType--}
```
public int getType()
```


Ottiene il tipo di questo oggetto valore di formattazione condizionale. Impostare il tipo su FormatConditionValueType.Min o FormatConditionValueType.Max imposterà automaticamente \"Value\" a null.

Vedi [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Ottiene il valore di questo oggetto valore di formattazione condizionale. Deve essere usato in congiunzione con Type.

**Remarks**

Se il valore è una stringa e inizia con \"=\", verrà elaborato come una formula, altrimenti lo elaboreremo come un valore semplice.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


Ottiene il flag Maggiore o Uguale. Usare solo per i set di icone, determina se questo valore soglia utilizza l'operatore maggiore o uguale. 'false' indica che viene usato 'maggiore' invece di 'maggiore o uguale'. Il valore predefinito è true.

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




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


Imposta il flag Maggiore o Uguale. Usare solo per i set di icone, determina se questo valore soglia utilizza l'operatore maggiore o uguale. 'false' indica che viene usato 'maggiore' invece di 'maggiore o uguale'. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Imposta il tipo di questo oggetto valore di formattazione condizionale. Impostare il tipo su FormatConditionValueType.Min o FormatConditionValueType.Max imposterà automaticamente \"Value\" a null.

Vedi [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Imposta il valore di questo oggetto valore di formattazione condizionale. Deve essere usato in congiunzione con Type.

**Remarks**

Se il valore è una stringa e inizia con \"=\", verrà elaborato come una formula, altrimenti lo elaboreremo come un valore semplice.

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

