---
title: "Slicer"
second_title: "Справочник API Aspose.Cells for Java"
description: "Краткое описание представления Slicer View."
type: docs
url: /ru/java/com.aspose.cells/slicer/
---

**Inheritance:**
java.lang.Object
```
public class Slicer
```

Краткое описание представления Slicer View.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         slicer.unselectItems(new String[] { "grape" });
         //do your business
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | Добавляет соединение PivotTable. |
| [clearFilter()](#clearFilter--) | Удалить фильтры |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Возвращает или задаёт описательную (альтернативную) строку текста объекта Slicer. |
| [getCaption()](#getCaption--) | Возвращает или задаёт подпись указанного слайсера. |
| [getCaptionVisible()](#getCaptionVisible--) | Возвращает или задаёт, видим ли заголовок, отображающий подпись слайсера. |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | Возвращает или задаёт ширину каждого столбца в слайсере в пунктах. |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | Получает ширину\\u807dкаждого столбца в\\u807dслайсере, в единицах\\u807dпикселей.\\u807d |
| [getFirstItemIndex()](#getFirstItemIndex--) | Указывает нулевой индекс первого элемента слайсера. |
| [getHeight()](#getHeight--) | Возвращает или задаёт высоту указанного слайсера в пунктах. |
| [getHeightPixel()](#getHeightPixel--) | Возвращает или задает высоту указанного среза, в пикселях. |
| [getLeftPixel()](#getLeftPixel--) | Возвращает или задает горизонтальное смещение формы среза от её левого столбца, в пикселях. |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | Указывает, включена ли блокировка соотношения сторон. |
| [getLockedPosition()](#getLockedPosition--) | Указывает, можно ли перемещать или изменять размер указанного среза с помощью пользовательского интерфейса. |
| [getName()](#getName--) | Возвращает или задает имя указанного среза |
| [getNumberOfColumns()](#getNumberOfColumns--) | Возвращает или задает количество столбцов в срезе. |
| [getParent()](#getParent--) | Возвращает объект [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) , содержащий этот срез. |
| [getPlacement()](#getPlacement--) | Представляет способ, которым объект рисунка привязан к находящимся под ним ячейкам. |
| [getRowHeight()](#getRowHeight--) | Возвращает или задает высоту каждой строки в указанном срезе в единицах пунктов. |
| [getRowHeightPixel()](#getRowHeightPixel--) | Возвращает или задает высоту каждой строки в указанном срезе, в единицах пикселей. |
| [getShape()](#getShape--) | Возвращает объект Shape, связанный с указанным срезом. |
| [getShowAllItems()](#getShowAllItems--) | Указывает, показывать ли все элементы, даже если данных нет или они удалены. |
| [getShowCaption()](#getShowCaption--) | Указывает, видим ли заголовок среза. |
| [getShowMissing()](#getShowMissing--) | Указывает, показывать ли элементы, удалённые из источника данных. |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--) | Указывает, показывать ли элементы, удалённые из источника данных. |
| [getSlicerCache()](#getSlicerCache--) | Возвращает объект SlicerCache, связанный с срезом. |
| [getSortOrderType()](#getSortOrderType--) | Указывает тип сортировки элементов. |
| [getStyleType()](#getStyleType--) | Укажите тип встроенного стиля среза. |
| [getTitle()](#getTitle--) | Указывает заголовок текущего объекта Slicer. |
| [getTopPixel()](#getTopPixel--) | Возвращает или задает вертикальное смещение формы среза от её верхней строки, в пикселях. |
| [getWidth()](#getWidth--) | Возвращает или задает ширину указанного среза, в пунктах. |
| [getWidthPixel()](#getWidthPixel--) | Возвращает или задает ширину указанного среза, в пикселях. |
| [getWorksheet()](#getWorksheet--) | Возвращает объект [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) , содержащий этот срез. |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | Указывает, заблокирована ли форма среза. |
| [isPrintable()](#isPrintable--) | Указывает, печатаем ли объект среза. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Обновление элементов среза из связанных сводных таблиц. |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | Удаляет связь с PivotTable. |
| [selectItems(String[] labels, boolean append)](#selectItems-java.lang.String---boolean-) | **Примечания** |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Возвращает или задаёт описательную (альтернативную) строку текста объекта Slicer. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Возвращает или задаёт подпись указанного слайсера. |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | Возвращает или задаёт, видим ли заголовок, отображающий подпись слайсера. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Возвращает или задаёт ширину каждого столбца в слайсере в пунктах. |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | Устанавливает ширину\u807dкаждого столбца в\u807dсрезе, в единицах\u807dпикселей.\u807d |
| [setFirstItemIndex(int value)](#setFirstItemIndex-int-) | Указывает нулевой индекс первого элемента слайсера. |
| [setHeight(double value)](#setHeight-double-) | Возвращает или задаёт высоту указанного слайсера в пунктах. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Возвращает или задает высоту указанного среза, в пикселях. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Возвращает или задает горизонтальное смещение формы среза от её левого столбца, в пикселях. |
| [setLocked(boolean value)](#setLocked-boolean-) | Указывает, заблокирована ли форма среза. |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | Указывает, включена ли блокировка соотношения сторон. |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | Указывает, можно ли перемещать или изменять размер указанного среза с помощью пользовательского интерфейса. |
| [setName(String value)](#setName-java.lang.String-) | Возвращает или задает имя указанного среза |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Возвращает или задает количество столбцов в срезе. |
| [setPlacement(int value)](#setPlacement-int-) | Представляет способ, которым объект рисунка привязан к находящимся под ним ячейкам. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Указывает, печатаем ли объект среза. |
| [setRowHeight(double value)](#setRowHeight-double-) | Возвращает или задает высоту каждой строки в указанном срезе в единицах пунктов. |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | Возвращает или задает высоту каждой строки в указанном срезе, в единицах пикселей. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Указывает, показывать ли все элементы, даже если данных нет или они удалены. |
| [setShowCaption(boolean value)](#setShowCaption-boolean-) | Указывает, видим ли заголовок среза. |
| [setShowMissing(boolean value)](#setShowMissing-boolean-) | Указывает, показывать ли элементы, удалённые из источника данных. |
| [setShowTypeOfItemsWithNoData(int value)](#setShowTypeOfItemsWithNoData-int-) | Указывает, показывать ли элементы, удалённые из источника данных. |
| [setSortOrderType(int value)](#setSortOrderType-int-) | Указывает тип сортировки элементов. |
| [setStyleType(int value)](#setStyleType-int-) | Укажите тип встроенного стиля среза. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Указывает заголовок текущего объекта Slicer. |
| [setTopPixel(int value)](#setTopPixel-int-) | Возвращает или задает вертикальное смещение формы среза от её верхней строки, в пикселях. |
| [setWidth(double value)](#setWidth-double-) | Возвращает или задает ширину указанного среза, в пунктах. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Возвращает или задает ширину указанного среза, в пикселях. |
| [toString()](#toString--) |  |
| [unselectItems(String[] labels)](#unselectItems-java.lang.String---) | Удалить выбранные метки фильтра. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```


Добавляет соединение PivotTable.

**Example**

```
         slicer.addPivotConnection(pivot);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Удалить фильтры

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Возвращает или задаёт описательную (альтернативную) строку текста объекта Slicer.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.getAlternativeText()](../../com.aspose.cells/shape\\#getAlternativeText--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```


Возвращает или задаёт подпись указанного слайсера.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```


Возвращает или задает, виден ли заголовок, отображающий подпись среза. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [getShowCaption()](../../com.aspose.cells/slicer\\#getShowCaption--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Возвращает или задаёт ширину каждого столбца в слайсере в пунктах.

**Example**

```
         slicer.setColumnWidth(80);
```

**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```


Получает ширину\\u807dкаждого столбца в\\u807dслайсере, в единицах\\u807dпикселей.\\u807d

**Example**

```
         slicer.setColumnWidthPixel(120);
```

**Returns:**
int
### getFirstItemIndex() {#getFirstItemIndex--}
```
public int getFirstItemIndex()
```


Указывает нулевой индекс первого элемента слайсера.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Возвращает или задаёт высоту указанного слайсера в пунктах.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.HeightPt. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Возвращает или задает высоту указанного среза, в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Height. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Возвращает или задает горизонтальное смещение формы среза от её левого столбца, в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Left. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```


Указывает, включена ли блокировка соотношения сторон.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\\#isAspectRatioLocked--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```


Указывает, можно ли перемещать или изменять размер указанного среза с помощью пользовательского интерфейса.

**Example**

```
         slicer.setLockedPosition(false);
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Возвращает или задает имя указанного среза

**Example**

```
         slicer.setName("slicer name");
```

**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Возвращает или задает количество столбцов в срезе. Значение по умолчанию — 1.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```


Возвращает объект [getWorksheet()](../../com.aspose.cells/slicer\\#getWorksheet--), содержащий этот срез. Только для чтения.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [getWorksheet()](../../com.aspose.cells/slicer\\#getWorksheet--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Представляет способ, которым объект рисунка привязан к находящимся под ним ячейкам. Свойство управляет размещением объекта на листе.

См. [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.getPlacement()](../../com.aspose.cells/shape\\#getPlacement--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Возвращает или задает высоту каждой строки в указанном срезе в единицах пунктов.

**Example**

```
         slicer.setRowHeight(20);
```

**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```


Возвращает или задает высоту каждой строки в указанном срезе, в единицах пикселей.

**Example**

```
         slicer.setRowHeightPixel(30);
```

**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```


Возвращает объект Shape, связанный с указанным срезом. Только для чтения.

**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Указывает, следует ли показывать все элементы, даже если данных нет или они удалены. Значение по умолчанию — true;

**Returns:**
boolean
### getShowCaption() {#getShowCaption--}
```
public boolean getShowCaption()
```


Указывает, виден ли заголовок среза. Значение по умолчанию — true.

**Example**

```
         slicer.setShowCaption(false);
```

**Returns:**
boolean
### getShowMissing() {#getShowMissing--}
```
public boolean getShowMissing()
```


Указывает, показывать ли элементы, удалённые из источника данных.

**Remarks**

Работает только когда [getShowAllItems()](../../com.aspose.cells/slicer\\#getShowAllItems--) равно true.

**Returns:**
boolean
### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}
```
public int getShowTypeOfItemsWithNoData()
```


Указывает, показывать ли элементы, удалённые из источника данных.

См. [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Работает только когда [getShowAllItems()](../../com.aspose.cells/slicer\\#getShowAllItems--) равно true.

**Returns:**
int
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```


Возвращает объект SlicerCache, связанный с срезом. Только для чтения.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getSortOrderType() {#getSortOrderType--}
```
public int getSortOrderType()
```


Указывает тип сортировки элементов.

См. [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```


Укажите тип встроенного стиля среза. Тип по умолчанию — SlicerStyleLight1.

См. [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Example**

```
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```

**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```


Указывает заголовок текущего объекта Slicer.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.getTitle()](../../com.aspose.cells/shape\\#getTitle--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Возвращает или задает вертикальное смещение формы среза от её верхней строки, в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Top. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Возвращает или задает ширину указанного среза, в пунктах.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.WidthPt. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Возвращает или задает ширину указанного среза, в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Width. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Возвращает объект [getWorksheet()](../../com.aspose.cells/slicer\\#getWorksheet--), содержащий этот срез. Только для чтения.

**Example**

```
         Worksheet currSheet = slicer.getParent();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Указывает, заблокирована ли форма среза.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.isLocked()](../../com.aspose.cells/shape\\#isLocked--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Указывает, печатаем ли объект среза.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.isPrintable()](../../com.aspose.cells/shape\\#isPrintable--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public void refresh()
```


Обновление элементов среза из связанных сводных таблиц.

**Example**

```
         slicer.refresh();
```

### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```


Удаляет связь с PivotTable.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |

### selectItems(String[] labels, boolean append) {#selectItems-java.lang.String---boolean-}
```
public void selectItems(String[] labels, boolean append)
```


**Remarks**

Если вы хотите выбрать все элементы, пожалуйста, используйте метод [clearFilter()](../../com.aspose.cells/slicer\\#clearFilter--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| метки | java.lang.String[] | Выбранные метки. |
| добавить | boolean | False означает только выбор этих меток и снятие выбора с остальных. True означает сохранение ранее выбранных элементов и выбор этих меток. |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Возвращает или задаёт описательную (альтернативную) строку текста объекта Slicer.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.getAlternativeText()](../../com.aspose.cells/shape\\#getAlternativeText--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Возвращает или задаёт подпись указанного слайсера.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```


Возвращает или задает, виден ли заголовок, отображающий подпись среза. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [getShowCaption()](../../com.aspose.cells/slicer\\#getShowCaption--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Возвращает или задаёт ширину каждого столбца в слайсере в пунктах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```


Устанавливает ширину\u807dкаждого столбца в\u807dсрезе, в единицах\u807dпикселей.\u807d

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFirstItemIndex(int value) {#setFirstItemIndex-int-}
```
public void setFirstItemIndex(int value)
```


Указывает нулевой индекс первого элемента слайсера.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Возвращает или задаёт высоту указанного слайсера в пунктах.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.HeightPt. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Возвращает или задает высоту указанного среза, в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Height. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


Возвращает или задает горизонтальное смещение формы среза от её левого столбца, в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Left. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Указывает, заблокирована ли форма среза.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.isLocked()](../../com.aspose.cells/shape\\#isLocked--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```


Указывает, включена ли блокировка соотношения сторон.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\\#isAspectRatioLocked--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```


Указывает, можно ли перемещать или изменять размер указанного среза с помощью пользовательского интерфейса.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Возвращает или задает имя указанного среза

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Возвращает или задает количество столбцов в срезе. Значение по умолчанию — 1.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Представляет способ, которым объект рисунка привязан к находящимся под ним ячейкам. Свойство управляет размещением объекта на листе.

См. [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.getPlacement()](../../com.aspose.cells/shape\\#getPlacement--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Указывает, печатаем ли объект среза.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.isPrintable()](../../com.aspose.cells/shape\\#isPrintable--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Возвращает или задает высоту каждой строки в указанном срезе в единицах пунктов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```


Возвращает или задает высоту каждой строки в указанном срезе, в единицах пикселей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Указывает, следует ли показывать все элементы, даже если данных нет или они удалены. Значение по умолчанию — true;

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowCaption(boolean value) {#setShowCaption-boolean-}
```
public void setShowCaption(boolean value)
```


Указывает, виден ли заголовок среза. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowMissing(boolean value) {#setShowMissing-boolean-}
```
public void setShowMissing(boolean value)
```


Указывает, показывать ли элементы, удалённые из источника данных.

**Remarks**

Работает только когда [getShowAllItems()](../../com.aspose.cells/slicer\\#getShowAllItems--) равно true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowTypeOfItemsWithNoData(int value) {#setShowTypeOfItemsWithNoData-int-}
```
public void setShowTypeOfItemsWithNoData(int value)
```


Указывает, показывать ли элементы, удалённые из источника данных.

См. [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Работает только когда [getShowAllItems()](../../com.aspose.cells/slicer\\#getShowAllItems--) равно true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSortOrderType(int value) {#setSortOrderType-int-}
```
public void setSortOrderType(int value)
```


Указывает тип сортировки элементов.

См. [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```


Укажите тип встроенного стиля среза. Тип по умолчанию — SlicerStyleLight1.

См. [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Указывает заголовок текущего объекта Slicer.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [Shape.getTitle()](../../com.aspose.cells/shape\\#getTitle--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Возвращает или задает вертикальное смещение формы среза от её верхней строки, в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Top. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Возвращает или задает ширину указанного среза, в пунктах.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.WidthPt. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Возвращает или задает ширину указанного среза, в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Width. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unselectItems(String[] labels) {#unselectItems-java.lang.String---}
```
public void unselectItems(String[] labels)
```


Удалить выбранные метки фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| метки | java.lang.String[] | Метки. |

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

