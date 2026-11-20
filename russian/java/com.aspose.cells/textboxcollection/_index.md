---
title: "TextBoxCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.cells/textboxcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TextBoxCollection extends CollectionBase
```

Инкапсулирует коллекцию объектов [TextBox](../../com.aspose.cells/textbox).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //get collection object
         TextBoxCollection textBoxCollection = workbook.getWorksheets().get(0).getTextBoxes();
         //add a textbox
         textBoxCollection.add(1, 1, 50, 100);
         for(TextBox tbox : (Iterable<TextBox>) textBoxCollection)
         {
             //do what you want
         }
 
         //do your business
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(int topRow, int leftColumn, int height, int width)](#add-int-int-int-int-) | Добавляет текстовое поле в коллекцию. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [clear()](#clear--) | Очищает все текстовые поля. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [TextBox](../../com.aspose.cells/textbox) по указанному индексу. |
| [get(String name)](#get-java.lang.String-) | Получает элемент [TextBox](../../com.aspose.cells/textbox) по имени. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удалить текстовое поле из файла. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int height, int width) {#add-int-int-int-int-}
```
public int add(int topRow, int leftColumn, int height, int width)
```


Добавляет текстовое поле в коллекцию.

**Example**

```
         //add a TextBox
         int index2 = textBoxCollection.add(1, 1, 50, 100);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| height | int | Высота textbox, в единицах пикселя. |
| width | int | Ширина textbox, в единицах пикселя. |

**Returns:**
int - индекс объекта [TextBox](../../com.aspose.cells/textbox).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Добавляет элемент в экземпляр CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Объект, который нужно добавить в экземпляр CollectionBase. |

**Returns:**
int — позиция, в которую был вставлен новый элемент.
### clear() {#clear--}
```
public void clear()
```


Очищает все текстовые поля.

**Example**

```
         //clear all textbox
         textBoxCollection.clear();
```

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Возвращает, содержит ли экземпляр этот объект

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | тестовый объект |

**Returns:**
boolean — содержит ли экземпляр этот объект
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
public TextBox get(int index)
```


Получает элемент [TextBox](../../com.aspose.cells/textbox) по указанному индексу.

**Example**

```
         int index = textBoxCollection.getCount() - 1;
         TextBox txb = textBoxCollection.get(index);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public TextBox get(String name)
```


Получает элемент [TextBox](../../com.aspose.cells/textbox) по имени.

**Example**

```
         String txtboxName = "textbox 1"; 
         TextBox txb2 = textBoxCollection.get(txtboxName);
         if(txb2 != null)
         {
             //do what you want
         }
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя текстового поля. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
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


Получает количество элементов, содержащихся в экземпляре CollectionBase.

**Returns:**
int — количество элементов, содержащихся в экземпляре CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Определяет индекс конкретного элемента в экземпляре CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Определяет индекс конкретного элемента в экземпляре CollectionBase. |

**Returns:**
int — индекс значения, если оно найдено в списке; иначе -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Возвращает перечислитель, который проходит по экземпляру CollectionBase.

**Returns:**
java.util.Iterator — итератор для экземпляра CollectionBase.
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


Удалить текстовое поле из файла.

**Example**

```
         int index3 = textBoxCollection.getCount() - 1;
         textBoxCollection.removeAt(index3);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс текстового поля. |

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

