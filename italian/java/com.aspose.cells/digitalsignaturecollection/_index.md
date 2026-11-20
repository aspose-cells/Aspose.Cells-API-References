---
title: "DigitalSignatureCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Fornisce una raccolta di firme digitali allegate a un documento."
type: docs
url: /it/java/com.aspose.cells/digitalsignaturecollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DigitalSignatureCollection implements Iterable
```

Fornisce una raccolta di firme digitali allegate a un documento.

**Example**

Il seguente esempio mostra come convalidare la firma digitale.

```
         //workbook from a signed source file
         Workbook signedWorkbook = new Workbook("signedFile.xlsx");
         //wb.IsDigitallySigned is true when the workbook is signed already.
         System.out.println(signedWorkbook.isDigitallySigned());
         //get digitalSignature collection from workbook
         DigitalSignatureCollection existingDsc = signedWorkbook.getDigitalSignature();
         for (DigitalSignature existingDs : (Iterable<DigitalSignature>) existingDsc)
         {
             System.out.println(existingDs.getComments());
             System.out.println(existingDs.getSignTime());
             System.out.println(existingDs.isValid());
         }
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DigitalSignatureCollection()](#DigitalSignatureCollection--) | Il costruttore di DigitalSignatureCollection. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(DigitalSignature digitalSignature)](#add-com.aspose.cells.DigitalSignature-) | Aggiungi una firma a DigitalSignatureCollection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Ottieni l'enumeratore per DigitalSignatureCollection, questo enumeratore consente l'iterazione sulla collezione |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignatureCollection() {#DigitalSignatureCollection--}
```
public DigitalSignatureCollection()
```


Il costruttore di DigitalSignatureCollection.

### add(DigitalSignature digitalSignature) {#add-com.aspose.cells.DigitalSignature-}
```
public void add(DigitalSignature digitalSignature)
```


Aggiungi una firma a DigitalSignatureCollection.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | Firma digitale nella collezione. |

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
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottieni l'enumeratore per DigitalSignatureCollection, questo enumeratore consente l'iterazione sulla collezione

**Returns:**
java.util.Iterator - L'enumeratore per l'iterazione.
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

