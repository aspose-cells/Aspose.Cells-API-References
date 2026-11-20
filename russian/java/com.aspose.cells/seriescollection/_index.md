---
title: "SeriesCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.cells/seriescollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```

Инкапсулирует коллекцию объектов [Series](../../com.aspose.cells/series).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [add(String dataArea, boolean isVertical)](#add-java.lang.String-boolean-) | Добавляет коллекцию [Series](../../com.aspose.cells/series) в диаграмму. |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | Добавляет коллекцию [Series](../../com.aspose.cells/series) в диаграмму. |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | Добавляет коллекцию [Series](../../com.aspose.cells/series) в диаграмму. |
| [changeColors(int type)](#changeColors-int-) | Устанавливает монохромную палитру для серий диаграммы. |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | Непосредственно изменяет порядок двух серий. |
| [clear()](#clear--) | Очищает коллекцию |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [Series](../../com.aspose.cells/series) по указанному индексу. |
| [getCategoryData()](#getCategoryData--) | Получает диапазон значений оси категорий. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [getSecondCategoryData()](#getSecondCategoryData--) | Получает диапазон значений второй оси категорий. |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | Получает элемент [Series](../../com.aspose.cells/series) по порядку. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [isColorVaried()](#isColorVaried--) | Отображает, изменяется ли цвет точек. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет серию по указанному индексу. |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | Устанавливает диапазон значений оси категорий. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Отображает, изменяется ли цвет точек. |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | Устанавливает диапазон значений второй оси категорий. |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | Устанавливает имена всех рядов в диаграмме. |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | Непосредственно изменяет порядок двух серий. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String dataArea, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String dataArea, boolean isVertical)
```


Добавляет коллекцию [Series](../../com.aspose.cells/series) в диаграмму.

**Remarks**


Если задаются данные в смежных ячейках, используйте двоеточие для их разделения. Например, $C$2:$C$5.

Если задаются данные в несмежных ячейках, используйте запятую для их разделения. Например: ($C$2,$D$5).

Этот метод просто обрабатывает как диапазон данных. Если вы хотите интеллектуально проверить метод ChartCollection.Add().


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dataArea | java.lang.String | Указывает значения, из которых строятся ряды данных |
| isVertical | boolean | Указывает, строить ли ряды из диапазона значений ячеек по строкам или по столбцам. Если true, [Series](../../com.aspose.cells/series) будет добавлен столбец за столбцом |

**Returns:**
int — возвращает первый индекс добавленного ASeries в NSeries.
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```


Добавляет коллекцию [Series](../../com.aspose.cells/series) в диаграмму.

**Remarks**


Если задаются данные в смежных ячейках, используйте двоеточие для их разделения. Например, $C$2:$C$5.

Если задаются данные в несмежных ячейках, используйте запятую для их разделения. Например, ($C$2,$D$5).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| area | java.lang.String | Указывает значения, из которых строятся ряды данных |
| isVertical | boolean | Указывает, строить ли ряды из диапазона значений ячеек по строкам или по столбцам. |
| checkLabels | boolean | Указывает, содержит ли диапазон имя ряда |

**Returns:**
int — возвращает первый индекс добавленного ASeries в NSeries.
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```


Добавляет коллекцию [Series](../../com.aspose.cells/series) в диаграмму.

**Remarks**


Если задаются данные в смежных ячейках, используйте двоеточие для их разделения. Например, R[1]C[1]:R[3]C[2].

Если задаются данные в смежных ячейках, используйте запятую для их разделения. Например, (R[1]C[1],R[3]C[2]).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| area | java.lang.String | Указывает значения, из которых строятся ряды данных |
| isVertical | boolean | Указывает, строить ли ряды из диапазона значений ячеек по строкам или по столбцам. |

**Returns:**
int — возвращает первый индекс добавленного ASeries в NSeries.
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```


Устанавливает монохромную палитру для серий диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype). Монохромный тип. |

### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```


Непосредственно изменяет порядок двух серий.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод SeriesCollection.SwapSeries. Этот метод будет удалён через 12 месяцев, начиная с июня 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceIndex | int | Текущий индекс |
| destIndex | int | Индекс назначения |

### clear() {#clear--}
```
public void clear()
```


Очищает коллекцию

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
public Series get(int index)
```


Получает элемент [Series](../../com.aspose.cells/series) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```


Получает диапазон значений оси категорий. Это может быть диапазон ячеек (например, "d1:e10") или последовательность значений (например, "\{2,6,8,10\}").

**Returns:**
java.lang.String
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
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```


Получает диапазон значений второй оси категорий. Это может быть диапазон ячеек (например, "d1:e10"), или последовательность значений (например, "\{2,6,8,10\}"). Действует только когда некоторые ряды построены на второй оси.

**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```


Получает элемент [Series](../../com.aspose.cells/series) по порядку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| order | int | Порядок серий |

**Returns:**
[Series](../../com.aspose.cells/series) - The element series
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
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Отображает, изменяется ли цвет точек.

**Remarks**

Работает только для круговой диаграммы или когда есть только одна серия.

**Returns:**
boolean
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


Удаляет серию по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |

### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```


Устанавливает диапазон значений оси категорий. Это может быть диапазон ячеек (например, "d1:e10") или последовательность значений (например, "\{2,6,8,10\}").

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Отображает, изменяется ли цвет точек.

**Remarks**

Работает только для круговой диаграммы или когда есть только одна серия.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```


Устанавливает диапазон значений второй оси категорий. Это может быть диапазон ячеек (например, "d1:e10"), или последовательность значений (например, "\{2,6,8,10\}"). Действует только когда некоторые серии построены на второй оси.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```


Устанавливает имена всех рядов в диаграмме.

**Remarks**


Если начальный индекс больше количества серий, метод вернётся и ничего не сделает.

Если задаются данные в смежных ячейках, используйте двоеточие для их разделения. Например, $C$2:$C$5.

Если задавать данные в смежных ячейках, используйте запятую для их разделения. Например, ($C$2,$D$5).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Индекс первой серии, для которой вы хотите задать имя. |
| area | java.lang.String | Указывает область для имени серии. |
| isVertical | boolean | >Указывает, строить ли серию из диапазона значений ячеек по строкам или по столбцам. |

### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```


Непосредственно изменяет порядок двух серий.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceIndex | int | Текущий индекс |
| destIndex | int | Индекс назначения |

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

