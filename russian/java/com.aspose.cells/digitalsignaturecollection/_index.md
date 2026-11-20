---
title: "DigitalSignatureCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Предоставляет коллекцию цифровых подписей, прикреплённых к документу."
type: docs
url: /ru/java/com.aspose.cells/digitalsignaturecollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DigitalSignatureCollection implements Iterable
```

Предоставляет коллекцию цифровых подписей, прикреплённых к документу.

**Example**

Следующий пример показывает, как проверить цифровую подпись.

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
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DigitalSignatureCollection()](#DigitalSignatureCollection--) | Конструктор DigitalSignatureCollection. |
## Методы

| Метод | Описание |
| --- | --- |
| [add(DigitalSignature digitalSignature)](#add-com.aspose.cells.DigitalSignature-) | Добавить одну подпись в DigitalSignatureCollection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Получить перечислитель для DigitalSignatureCollection, этот перечислитель позволяет выполнять итерацию по коллекции |
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


Конструктор DigitalSignatureCollection.

### add(DigitalSignature digitalSignature) {#add-com.aspose.cells.DigitalSignature-}
```
public void add(DigitalSignature digitalSignature)
```


Добавить одну подпись в DigitalSignatureCollection.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | Цифровая подпись в коллекции. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
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


Получить перечислитель для DigitalSignatureCollection, этот перечислитель позволяет выполнять итерацию по коллекции

**Returns:**
java.util.Iterator - перечислитель для итерации.
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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

