---
title: "DigitalSignatureCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Sammlung digitaler Signaturen bereit, die an ein Dokument angehängt sind."
type: docs
url: /de/java/com.aspose.cells/digitalsignaturecollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DigitalSignatureCollection implements Iterable
```

Stellt eine Sammlung digitaler Signaturen bereit, die an ein Dokument angehängt sind.

**Example**

Das folgende Beispiel zeigt, wie man eine digitale Signatur validiert.

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
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DigitalSignatureCollection()](#DigitalSignatureCollection--) | Der Konstruktor von DigitalSignatureCollection. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(DigitalSignature digitalSignature)](#add-com.aspose.cells.DigitalSignature-) | Füge eine Signatur zu DigitalSignatureCollection hinzu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Erhalte den Enumerator für DigitalSignatureCollection, dieser Enumerator ermöglicht die Iteration über die Sammlung. |
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


Der Konstruktor von DigitalSignatureCollection.

### add(DigitalSignature digitalSignature) {#add-com.aspose.cells.DigitalSignature-}
```
public void add(DigitalSignature digitalSignature)
```


Füge eine Signatur zu DigitalSignatureCollection hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | Digitale Signatur in der Sammlung. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Erhalte den Enumerator für DigitalSignatureCollection, dieser Enumerator ermöglicht die Iteration über die Sammlung.

**Returns:**
java.util.Iterator - Der Enumerator zur Iteration.
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

