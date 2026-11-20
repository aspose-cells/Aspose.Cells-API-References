---
title: "ExternalLinkCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет коллекцию внешних ссылок в книге."
type: docs
url: /ru/java/com.aspose.cells/externallinkcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```

Представляет коллекцию внешних ссылок в книге.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Change external link data source
         workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | Добавить внешнюю ссылку. |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | Добавляет внешнюю ссылку. |
| [clear()](#clear--) | Удаляет все внешние ссылки. |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | Удаляет все внешние ссылки. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [ExternalLink](../../com.aspose.cells/externallink) по указанному индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, фактически содержащихся в коллекции. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Получить перечислитель, который перебирает эту коллекцию. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет указанную внешнюю ссылку из рабочей книги. |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | Удаляет указанную внешнюю ссылку из рабочей книги. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```


Добавить внешнюю ссылку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype). Тип каталога имени файла. |
| fileName | java.lang.String | имя файла. |
| sheetNames | java.lang.String[] | Все имена листов внешнего файла. |

**Returns:**
int - Позиция внешнего имени в этом списке.
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```


Добавляет внешнюю ссылку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя внешнего файла. |
| sheetNames | java.lang.String[] | Все имена листов внешнего файла. |

**Returns:**
int - Позиция внешнего имени в этом списке.
### clear() {#clear--}
```
public void clear()
```


Удаляет все внешние ссылки.

**Remarks**

При удалении внешних ссылок все формулы, которые ссылаются на них, также будут удалены, потому что ссылки становятся недействительными.

### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```


Удаляет все внешние ссылки.

**Remarks**

Если требуется обновить ссылки, эти ссылки внешних ссылок в формулах будут изменены на текущую книгу, если это возможно. Например, исходная формула одной ячейки выглядит так "='externalsource.xlam'!customfunction()", после удаления внешних ссылок формула станет "=customfunction()"; Когда исходная формула выглядит так "='[externalsource.xlam]Sheet1'!$A$1", в зависимости от того, существует ли лист с именем "Sheet1" в текущей книге: если да, формула станет "=Sheet1!$A$1"; если нет, формула станет "=\#REF!$A$1".

Если обновление ссылок не требуется, все формулы со ссылками на внешние ссылки также будут удалены, потому что эти ссылки становятся недействительными.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Нужно ли обновлять все ссылки внешних ссылок в формулах на ссылки текущей книги. |

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
### get(int index) {#get-int-}
```
public ExternalLink get(int index)
```


Получает элемент [ExternalLink](../../com.aspose.cells/externallink) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Получает количество элементов, фактически содержащихся в коллекции.

**Returns:**
int
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


Получить перечислитель, который перебирает эту коллекцию.

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет указанную внешнюю ссылку из рабочей книги.

**Remarks**

При удалении внешней ссылки все формулы, которые ссылаются на неё, также будут удалены, потому что ссылки становятся недействительными.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс внешней ссылки, которую нужно удалить. |

### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```


Удаляет указанную внешнюю ссылку из рабочей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс внешней ссылки, которую нужно удалить. |
| updateReferencesAsLocal | boolean | Нужно ли обновлять все ссылки данной внешней ссылки на ссылки текущей книги. См. [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) для получения более подробной информации об этом параметре. |

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

