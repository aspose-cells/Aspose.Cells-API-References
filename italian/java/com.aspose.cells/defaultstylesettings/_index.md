---
title: "DefaultStyleSettings"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Impostazioni per i valori predefiniti delle proprietà di stile delle cartelle di lavoro."
type: docs
url: /it/java/com.aspose.cells/defaultstylesettings/
---

**Inheritance:**
java.lang.Object
```
public class DefaultStyleSettings
```

Impostazioni per i valori predefiniti delle proprietà di stile della cartella di lavoro.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInPreference()](#getBuiltInPreference--) | Indica se la proprietà del formato numerico è preferibile quando lo stile definisce sia un numero incorporato sia un modello personalizzato. |
| [getClass()](#getClass--) |  |
| [getFontName()](#getFontName--) | Restituisce il nome del carattere predefinito per la cartella di lavoro |
| [getFontSize()](#getFontSize--) | Restituisce la dimensione standard del carattere predefinita per la cartella di lavoro. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Restituisce il valore predefinito per l'allineamento orizzontale |
| [getVerticalAlignment()](#getVerticalAlignment--) | Restituisce il valore predefinito per l'allineamento verticale |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuiltInPreference(boolean value)](#setBuiltInPreference-boolean-) | Indica se la proprietà del formato numerico è preferibile quando lo stile definisce sia un numero incorporato sia un modello personalizzato. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Imposta il nome del carattere predefinito per la cartella di lavoro |
| [setFontSize(double value)](#setFontSize-double-) | Imposta la dimensione del carattere standard predefinita per la cartella di lavoro. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Imposta il valore predefinito per l'allineamento orizzontale |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Imposta il valore predefinito per l'allineamento verticale |
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
### getBuiltInPreference() {#getBuiltInPreference--}
```
public boolean getBuiltInPreference()
```


Indica se la proprietà per il formato numerico è preferibile quando lo stile definisce sia un numero incorporato sia un modello personalizzato. Il valore predefinito è false, il che significa che per impostazione predefinita verrà utilizzato il modello personalizzato per formattare i valori, purché non sia vuoto per uno stile.

**Remarks**

Durante il caricamento di una cartella di lavoro da un file modello esistente, è possibile che per uno stile siano definiti sia un numero incorporato sia un modello personalizzato. Questa proprietà determina se utilizzare il numero incorporato o il modello personalizzato durante la formattazione dei valori con lo stile.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontName() {#getFontName--}
```
public String getFontName()
```


Restituisce il nome del carattere predefinito per la cartella di lavoro

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Restituisce la dimensione standard del carattere predefinita per la cartella di lavoro.

**Returns:**
double
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Restituisce il valore predefinito per l'allineamento orizzontale

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Restituisce il valore predefinito per l'allineamento verticale

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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




### setBuiltInPreference(boolean value) {#setBuiltInPreference-boolean-}
```
public void setBuiltInPreference(boolean value)
```


Indica se la proprietà per il formato numerico è preferibile quando lo stile definisce sia un numero incorporato sia un modello personalizzato. Il valore predefinito è false, il che significa che per impostazione predefinita verrà utilizzato il modello personalizzato per formattare i valori, purché non sia vuoto per uno stile.

**Remarks**

Durante il caricamento di una cartella di lavoro da un file modello esistente, è possibile che per uno stile siano definiti sia un numero incorporato sia un modello personalizzato. Questa proprietà determina se utilizzare il numero incorporato o il modello personalizzato durante la formattazione dei valori con lo stile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Imposta il nome del carattere predefinito per la cartella di lavoro

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFontSize(double value) {#setFontSize-double-}
```
public void setFontSize(double value)
```


Imposta la dimensione del carattere standard predefinita per la cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Imposta il valore predefinito per l'allineamento orizzontale

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Imposta il valore predefinito per l'allineamento verticale

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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

