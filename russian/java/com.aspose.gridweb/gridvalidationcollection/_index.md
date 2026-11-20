---
title: "GridValidationCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.gridweb/gridvalidationcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```

Инкапсулирует коллекцию объектов [GridValidation](../../com.aspose.gridweb/gridvalidation).
## Методы

| Метод | Описание |
| --- | --- |
| [add()](#add--) | Добавьте [GridValidation](../../com.aspose.gridweb/gridvalidation) в коллекцию. |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | Добавляет проверку данных в коллекцию. |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | Добавьте [GridValidation](../../com.aspose.gridweb/gridvalidation) в коллекцию. |
| [add(int row, int column)](#add-int-int-) | Добавьте [GridValidation](../../com.aspose.gridweb/gridvalidation) в коллекцию. Проверка применяется к указанной ячейке. |
| [add(String cellname)](#add-java.lang.String-) | Добавьте [GridValidation](../../com.aspose.gridweb/gridvalidation) в коллекцию. Проверка применяется к указанной ячейке. |
| [clear()](#clear--) | Очищает все проверки. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [GridValidation](../../com.aspose.gridweb/gridvalidation) по указанному индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает размер перечислителя |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | Получает проверку, примененную к указанной ячейке. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет проверку по указанному индексу. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```


Добавьте [GridValidation](../../com.aspose.gridweb/gridvalidation) в коллекцию.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод GridValidationCollection.Add(row,col). Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2015 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```


Добавляет проверку данных в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Область, содержащая эту проверку. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```


Добавьте [GridValidation](../../com.aspose.gridweb/gridvalidation) в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | Объект проверки. |

**Returns:**
int — индекс объекта [GridValidation](../../com.aspose.gridweb/gridvalidation).
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```


Добавьте [GridValidation](../../com.aspose.gridweb/gridvalidation) в коллекцию. Проверка применяется к указанной ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```


Добавьте [GridValidation](../../com.aspose.gridweb/gridvalidation) в коллекцию. Проверка применяется к указанной ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellname | java.lang.String | имя ячейки. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```


Очищает все проверки.

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
public GridValidation get(int index)
```


Получает элемент [GridValidation](../../com.aspose.gridweb/gridvalidation) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
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


Получает размер перечислителя

**Returns:**
int
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```


Получает проверку, примененную к указанной ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет проверку по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

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

