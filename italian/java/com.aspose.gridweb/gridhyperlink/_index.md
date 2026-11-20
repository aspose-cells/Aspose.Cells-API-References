---
title: "GridHyperlink"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un collegamento ipertestuale."
type: docs
url: /it/java/com.aspose.gridweb/gridhyperlink/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlink
```

Incapsula l'oggetto che rappresenta un collegamento ipertestuale.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Rappresenta l'indirizzo di un collegamento ipertestuale. |
| [getAltText()](#getAltText--) | Ottiene il testo alternativo per il collegamento immagine, si prega di notare che questo è un attributo di estensione e non può essere conservato nel file Excel. |
| [getArea()](#getArea--) | Ottiene l'intervallo del collegamento ipertestuale. |
| [getClass()](#getClass--) |  |
| [getCommand()](#getCommand--) | Restituisce o imposta il testo del valore del comando definito dall'utente per il collegamento ipertestuale specificato. |
| [getDiscardInput()](#getDiscardInput--) | Indica se scartare l'input dell'utente nel browser client quando l'utente clicca su questo collegamento ipertestuale CellCommand. |
| [getImageURL()](#getImageURL--) | Ottiene l'URL dell'immagine per il collegamento, non esistono proprietà imageurl nel collegamento ipertestuale, quindi si utilizza effettivamente TextToDisplay per registrare questo valore; TextToDisplay verrà impostato a <img src=value> così cambierà il valore di TextToDisplay. |
| [getScreenTip()](#getScreenTip--) | Restituisce o imposta il testo del suggerimento per il collegamento ipertestuale specificato. |
| [getTarget()](#getTarget--) | Ottiene il tipo di destinazione del collegamento web, si prega di notare che questo è un attributo di estensione e non può essere conservato nel file Excel. |
| [getTextToDisplay()](#getTextToDisplay--) | Rappresenta il testo da visualizzare per il collegamento ipertestuale specificato. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Rappresenta l'indirizzo di un collegamento ipertestuale. |
| [setAltText(String value)](#setAltText-java.lang.String-) | Imposta il testo alternativo per il collegamento immagine, si prega di notare che questo è un attributo di estensione e non può essere conservato nel file Excel. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Restituisce o imposta il testo del valore del comando definito dall'utente per il collegamento ipertestuale specificato. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Indica se scartare l'input dell'utente nel browser client quando l'utente clicca su questo collegamento ipertestuale CellCommand. |
| [setImageURL(String value)](#setImageURL-java.lang.String-) | Imposta l'URL dell'immagine per il collegamento, non esistono proprietà imageurl nel collegamento ipertestuale, quindi si utilizza effettivamente TextToDisplay per registrare questo valore; TextToDisplay verrà impostato a <img src=value> così cambierà il valore di TextToDisplay. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Restituisce o imposta il testo del suggerimento per il collegamento ipertestuale specificato. |
| [setTarget(String value)](#setTarget-java.lang.String-) | Imposta il tipo di destinazione del collegamento web, si prega di notare che questo è un attributo di estensione e non può essere conservato nel file Excel. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Rappresenta il testo da visualizzare per il collegamento ipertestuale specificato. |
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
### getAddress() {#getAddress--}
```
public String getAddress()
```


Rappresenta l'indirizzo di un collegamento ipertestuale.

**Returns:**
java.lang.String
### getAltText() {#getAltText--}
```
public String getAltText()
```


Ottiene il testo alternativo per il collegamento immagine, si prega di notare che questo è un attributo di estensione e non può essere conservato nel file Excel.

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public GridCellArea getArea()
```


Ottiene l'intervallo del collegamento ipertestuale.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommand() {#getCommand--}
```
public String getCommand()
```


Restituisce o imposta il testo del valore del comando definito dall'utente per il collegamento ipertestuale specificato.

**Returns:**
java.lang.String
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Indica se scartare l'input dell'utente nel browser client quando l'utente clicca su questo collegamento ipertestuale CellCommand. Potrebbe essere usato come azione di "undo".

**Returns:**
boolean
### getImageURL() {#getImageURL--}
```
public String getImageURL()
```


Ottiene l'URL dell'immagine per il collegamento, non esistono proprietà imageurl nel collegamento ipertestuale, quindi si utilizza effettivamente TextToDisplay per registrare questo valore; TextToDisplay verrà impostato a <img src=value> così cambierà il valore di TextToDisplay.

**Returns:**
java.lang.String
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


Restituisce o imposta il testo del suggerimento per il collegamento ipertestuale specificato.

**Returns:**
java.lang.String
### getTarget() {#getTarget--}
```
public String getTarget()
```


Ottiene il tipo di destinazione del collegamento web, si prega di notare che questo è un attributo di estensione e non può essere conservato nel file Excel.

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


Rappresenta il testo da visualizzare per il collegamento ipertestuale specificato. Il valore predefinito è l'indirizzo del collegamento ipertestuale.

**Returns:**
java.lang.String
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




### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```


Rappresenta l'indirizzo di un collegamento ipertestuale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAltText(String value) {#setAltText-java.lang.String-}
```
public void setAltText(String value)
```


Imposta il testo alternativo per il collegamento immagine, si prega di notare che questo è un attributo di estensione e non può essere conservato nel file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Restituisce o imposta il testo del valore del comando definito dall'utente per il collegamento ipertestuale specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


Indica se scartare l'input dell'utente nel browser client quando l'utente clicca su questo collegamento ipertestuale CellCommand. Potrebbe essere usato come azione di "undo".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setImageURL(String value) {#setImageURL-java.lang.String-}
```
public void setImageURL(String value)
```


Imposta l'URL dell'immagine per il collegamento, non esistono proprietà imageurl nel collegamento ipertestuale, quindi si utilizza effettivamente TextToDisplay per registrare questo valore; TextToDisplay verrà impostato a <img src=value> così cambierà il valore di TextToDisplay.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


Restituisce o imposta il testo del suggerimento per il collegamento ipertestuale specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTarget(String value) {#setTarget-java.lang.String-}
```
public void setTarget(String value)
```


Imposta il tipo di destinazione del collegamento web, si prega di notare che questo è un attributo di estensione e non può essere conservato nel file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


Rappresenta il testo da visualizzare per il collegamento ipertestuale specificato. Il valore predefinito è l'indirizzo del collegamento ipertestuale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

