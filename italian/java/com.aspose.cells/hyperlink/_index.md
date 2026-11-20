---
title: "Collegamento ipertestuale"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un collegamento ipertestuale."
type: docs
url: /it/java/com.aspose.cells/hyperlink/
---

**Inheritance:**
java.lang.Object
```
public class Hyperlink
```

Incapsula l'oggetto che rappresenta un collegamento ipertestuale.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a hyperlink to a URL at "A1" cell
         int index = worksheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
         //Getting a Hyperlink by index.
         Hyperlink hyperlink = worksheet.getHyperlinks().get(index);
         //Setting display text of this hyperlink.
         hyperlink.setTextToDisplay("Aspose");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [delete()](#delete--) | Elimina questo collegamento ipertestuale |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Rappresenta l'indirizzo di un collegamento ipertestuale. |
| [getArea()](#getArea--) | Ottiene l'intervallo del collegamento ipertestuale. |
| [getClass()](#getClass--) |  |
| [getLinkType()](#getLinkType--) | Ottiene il tipo di collegamento. |
| [getScreenTip()](#getScreenTip--) | Restituisce o imposta il testo del suggerimento per il collegamento ipertestuale specificato. |
| [getTextToDisplay()](#getTextToDisplay--) | Rappresenta il testo da visualizzare per il collegamento ipertestuale specificato. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Rappresenta l'indirizzo di un collegamento ipertestuale. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Restituisce o imposta il testo del suggerimento per il collegamento ipertestuale specificato. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Rappresenta il testo da visualizzare per il collegamento ipertestuale specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### delete() {#delete--}
```
public void delete()
```


Elimina questo collegamento ipertestuale

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
### getArea() {#getArea--}
```
public CellArea getArea()
```


Ottiene l'intervallo del collegamento ipertestuale.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLinkType() {#getLinkType--}
```
public int getLinkType()
```


Ottiene il tipo di collegamento.

Vedi [TargetModeType](../../com.aspose.cells/targetmodetype).

**Returns:**
int
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


Restituisce o imposta il testo del suggerimento per il collegamento ipertestuale specificato.

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

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


Restituisce o imposta il testo del suggerimento per il collegamento ipertestuale specificato.

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

