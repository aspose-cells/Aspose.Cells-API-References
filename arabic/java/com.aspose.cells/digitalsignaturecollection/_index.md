---
title: "DigitalSignatureCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يوفر مجموعة من التوقيعات الرقمية المرفقة بالمستند."
type: docs
url: /ar/java/com.aspose.cells/digitalsignaturecollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DigitalSignatureCollection implements Iterable
```

يوفر مجموعة من التوقيعات الرقمية المرفقة بالمستند.

**Example**

المثال التالي يوضح كيفية التحقق من صحة التوقيع الرقمي.

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
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DigitalSignatureCollection()](#DigitalSignatureCollection--) | المُنشئ الخاص بـ DigitalSignatureCollection. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(DigitalSignature digitalSignature)](#add-com.aspose.cells.DigitalSignature-) | أضف توقيعًا واحدًا إلى DigitalSignatureCollection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | احصل على المكرّر لـ DigitalSignatureCollection، هذا المكرّر يتيح التكرار عبر المجموعة |
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


المُنشئ الخاص بـ DigitalSignatureCollection.

### add(DigitalSignature digitalSignature) {#add-com.aspose.cells.DigitalSignature-}
```
public void add(DigitalSignature digitalSignature)
```


أضف توقيعًا واحدًا إلى DigitalSignatureCollection.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | التوقيع الرقمي في المجموعة. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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


احصل على المكرّر لـ DigitalSignatureCollection، هذا المكرّر يتيح التكرار عبر المجموعة

**Returns:**
java.util.Iterator - المكرّر للتكرار.
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

