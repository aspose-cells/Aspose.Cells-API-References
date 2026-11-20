---
title: "CellsDataTableFactory"
second_title: "Справочник API Aspose.Cells for Java"
description: "Утилита для создания ICellsDataTable из пользовательских объектов для удобства пользователей."
type: docs
url: /ru/java/com.aspose.cells/cellsdatatablefactory/
---

**Inheritance:**
java.lang.Object
```
public class CellsDataTableFactory
```

Утилита для создания ICellsDataTable из пользовательских объектов для удобства пользователя.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getInstance(double[] vals, boolean vertial)](#getInstance-double---boolean-) | Создаёт ICellsDataTable из заданной последовательности значений double. |
| [getInstance(double[] vals, String[] columnNames)](#getInstance-double---java.lang.String---) | Создаёт ICellsDataTable из заданной последовательности значений double. |
| [getInstance(double[][] vals)](#getInstance-double-----) | Создаёт ICellsDataTable из заданного двумерного массива. |
| [getInstance(int[] vals, boolean vertial)](#getInstance-int---boolean-) | Создаёт ICellsDataTable из заданной последовательности целочисленных значений. |
| [getInstance(int[] vals, String[] columnNames)](#getInstance-int---java.lang.String---) | Создаёт ICellsDataTable из заданной последовательности целочисленных значений. |
| [getInstance(int[][] vals)](#getInstance-int-----) | Создаёт ICellsDataTable из заданного двумерного массива. |
| [getInstance(Object[] vals, boolean vertial)](#getInstance-java.lang.Object---boolean-) | Создаёт ICellsDataTable из заданной последовательности объектов. |
| [getInstance(Object[] vals, String[] columnNames)](#getInstance-java.lang.Object---java.lang.String---) | Создаёт ICellsDataTable из заданной последовательности объектов. |
| [getInstance(Object[][] vals)](#getInstance-java.lang.Object-----) | Создаёт ICellsDataTable из заданного двумерного массива. |
| [getInstance(Object[][] vals, boolean hasHeader, String[] columnNames)](#getInstance-java.lang.Object-----boolean-java.lang.String---) | Создаёт ICellsDataTable из заданной последовательности объектов. |
| [getInstance(Collection collection)](#getInstance-java.util.Collection-) | Создаёт ICellsDataTable из заданной коллекции. |
| [getInstance(Collection collection, boolean hasHeader)](#getInstance-java.util.Collection-boolean-) | Создаёт ICellsDataTable из заданной коллекции. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getInstance(double[] vals, boolean vertial) {#getInstance-double---boolean-}
```
public ICellsDataTable getInstance(double[] vals, boolean vertial)
```


Создаёт ICellsDataTable из заданной последовательности значений double.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | double[] | значения double для построения таблицы |
| vertial | boolean | определяет, строить таблицу по значениям double vertiacally(true) или horizontallly(false) |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(double[] vals, String[] columnNames) {#getInstance-double---java.lang.String---}
```
public ICellsDataTable getInstance(double[] vals, String[] columnNames)
```


Создаёт ICellsDataTable из заданной последовательности значений double.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | double[] | значения double для построения таблицы |
| columnNames | java.lang.String[] | Имена столбцов таблицы. Его длина может быть только 1(создать таблицу по double values вертикально) или длина double values(создать таблицу по double values горизонтально) |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(double[][] vals) {#getInstance-double-----}
```
public ICellsDataTable getInstance(double[][] vals)
```


Создаёт ICellsDataTable из заданного двумерного массива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | double[][] | значения double для построения таблицы |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(int[] vals, boolean vertial) {#getInstance-int---boolean-}
```
public ICellsDataTable getInstance(int[] vals, boolean vertial)
```


Создаёт ICellsDataTable из заданной последовательности целочисленных значений.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | int[] | int значения для построения таблицы |
| vertial | boolean | нужно ли построить таблицу по int values вертикально(true) или горизонтально(false) |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(int[] vals, String[] columnNames) {#getInstance-int---java.lang.String---}
```
public ICellsDataTable getInstance(int[] vals, String[] columnNames)
```


Создаёт ICellsDataTable из заданной последовательности целочисленных значений.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | int[] | int значения для построения таблицы |
| columnNames | java.lang.String[] | Имена столбцов таблицы. Его длина может быть только 1(создать таблицу по int values вертикально) или длина int values(создать таблицу по int values горизонтально) |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(int[][] vals) {#getInstance-int-----}
```
public ICellsDataTable getInstance(int[][] vals)
```


Создаёт ICellsDataTable из заданного двумерного массива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | int[][] | int значения для построения таблицы |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[] vals, boolean vertial) {#getInstance-java.lang.Object---boolean-}
```
public ICellsDataTable getInstance(Object[] vals, boolean vertial)
```


Создаёт ICellsDataTable из заданной последовательности объектов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | java.lang.Object[] | объекты для построения таблицы |
| vertial | boolean | нужно ли построить таблицу по объектам вертикально(true) или горизонтально(false) |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[] vals, String[] columnNames) {#getInstance-java.lang.Object---java.lang.String---}
```
public ICellsDataTable getInstance(Object[] vals, String[] columnNames)
```


Создаёт ICellsDataTable из заданной последовательности объектов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | java.lang.Object[] | объекты для построения таблицы |
| columnNames | java.lang.String[] | Имена столбцов таблицы. Его длина может быть только 1(создать таблицу по objects вертикально) или длина objects(создать таблицу по objects горизонтально) |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[][] vals) {#getInstance-java.lang.Object-----}
```
public ICellsDataTable getInstance(Object[][] vals)
```


Создаёт ICellsDataTable из заданного двумерного массива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | java.lang.Object[][] | объекты для построения таблицы |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[][] vals, boolean hasHeader, String[] columnNames) {#getInstance-java.lang.Object-----boolean-java.lang.String---}
```
public ICellsDataTable getInstance(Object[][] vals, boolean hasHeader, String[] columnNames)
```


Создаёт ICellsDataTable из заданной последовательности объектов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | java.lang.Object[][] | объекты для построения таблицы |
| hasHeader | boolean | Указывает, является ли первая строка строкой заголовка. |
| columnNames | java.lang.String[] | Имена столбцов таблицы. Его длина может быть только 1(создать таблицу по objects вертикально) или длина objects(создать таблицу по objects горизонтально) |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Collection collection) {#getInstance-java.util.Collection-}
```
public ICellsDataTable getInstance(Collection collection)
```


Создаёт ICellsDataTable из заданной коллекции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| collection | java.util.Collection | коллекция для построения таблицы |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Collection collection, boolean hasHeader) {#getInstance-java.util.Collection-boolean-}
```
public ICellsDataTable getInstance(Collection collection, boolean hasHeader)
```


Создаёт ICellsDataTable из заданной коллекции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| collection | java.util.Collection | коллекция для построения таблицы |
| hasHeader | boolean | Указывает, является ли первая строка заголовком |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
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

