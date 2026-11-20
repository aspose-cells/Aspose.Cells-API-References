---
title: "Timeline"
second_title: "Справочник API Aspose.Cells for Java"
description: "Краткое описание представления Timeline. Из‑за того, что MS Excel 2003 не поддерживает Timeline."
type: docs
url: /ru/java/com.aspose.cells/timeline/
---

**Inheritance:**
java.lang.Object
```
public class Timeline
```

Краткое описание представления Timeline. Из‑за MS Excel Excel 2003 не поддерживает Timeline.

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
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
         //Add time line based on date field.
         int index = sheet.getTimelines().add(pivot, "E1","date");
         Timeline timeline = sheet.getTimelines().get(index);
 
         //do your business
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | Получает подпись этого Timeline. |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | Текущий уровень времени Timeline. |
| [getHeightPixel()](#getHeightPixel--) | Возвращает или задает высоту указанного timeline в пикселях. |
| [getLeftPixel()](#getLeftPixel--) | Возвращает или задает горизонтальное смещение формы timeline от её левого столбца в пикселях. |
| [getName()](#getName--) | Возвращает или задает имя указанного Timeline. |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--) | Получает выбранный диапазон даты и времени. |
| [getSelectionLevel()](#getSelectionLevel--) | Получает уровень времени, на котором была сделана текущая выборка для Timeline. |
| [getShape()](#getShape--) | Возвращает объект [TimelineShape](../../com.aspose.cells/timelineshape), связанный с этим Timeline. |
| [getShowHeader()](#getShowHeader--) | Указывает, следует ли отображать заголовок этого timeline. |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | Указывает, следует ли отображать горизонтальную полосу прокрутки. |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | Указывает, следует ли отображать метку выбора. |
| [getShowTimeLevel()](#getShowTimeLevel--) | Указывает, следует ли отображать выпадающий список выбора уровня времени. |
| [getStartDate()](#getStartDate--) | Получает дату начала позиции прокрутки временного интервала этого [Timeline](../../com.aspose.cells/timeline). |
| [getTopPixel()](#getTopPixel--) | Возвращает или задает вертикальное смещение формы timeline от её верхней строки в пикселях. |
| [getWidthPixel()](#getWidthPixel--) | Возвращает или задает ширину указанного timeline в пикселях. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(DateTime start, DateTime end, boolean calculate)](#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-) | Выберите элемент между датой и временем. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Задает подпись этого Timeline. |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | Текущий уровень времени Timeline. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Возвращает или задает высоту указанного timeline в пикселях. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Возвращает или задает горизонтальное смещение формы timeline от её левого столбца в пикселях. |
| [setName(String value)](#setName-java.lang.String-) | Возвращает или задает имя указанного Timeline. |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | Задает уровень времени, на котором была сделана текущая выборка для Timeline. |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | Указывает, следует ли отображать заголовок этого timeline. |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | Указывает, следует ли отображать горизонтальную полосу прокрутки. |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | Указывает, следует ли отображать метку выбора. |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | Указывает, следует ли отображать выпадающий список выбора уровня времени. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Задает дату начала позиции прокрутки временного интервала этого [Timeline](../../com.aspose.cells/timeline). |
| [setTopPixel(int value)](#setTopPixel-int-) | Возвращает или задает вертикальное смещение формы timeline от её верхней строки в пикселях. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Возвращает или задает ширину указанного timeline в пикселях. |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


Получает подпись этого Timeline.

**Example**

```
         //Set the caption of this Timeline.
         timeline.setCaption("timeline caption test");
```

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


Текущий уровень времени Timeline.

Смотрите [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Возвращает или задает высоту указанного timeline в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Height. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Возвращает или задает горизонтальное смещение формы timeline от её левого столбца в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Left. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Возвращает или задает имя указанного Timeline.

**Example**

```
         //Set the name of the specified Timeline.
         timeline.setName("timeline name test");
```

**Returns:**
java.lang.String
### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}
```
public DateTime[] getSelectedDateTimeRange()
```


Получает выбранный диапазон даты и времени.

**Returns:**
com.aspose.cells.DateTime[] -
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


Получает уровень времени, на котором была сделана текущая выборка для Timeline.

Смотрите [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


Возвращает объект [TimelineShape](../../com.aspose.cells/timelineshape), связанный с этим Timeline.

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


Указывает, следует ли отображать заголовок этого timeline.

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


Указывает, следует ли отображать горизонтальную полосу прокрутки.

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


Указывает, следует ли отображать метку выбора.

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


Указывает, следует ли отображать выпадающий список выбора уровня времени.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Получает дату начала позиции прокрутки временного интервала этого [Timeline](../../com.aspose.cells/timeline).

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Возвращает или задает вертикальное смещение формы timeline от её верхней строки в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Top. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Возвращает или задает ширину указанного timeline в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Width. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
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




### select(DateTime start, DateTime end, boolean calculate) {#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-}
```
public void select(DateTime start, DateTime end, boolean calculate)
```


Выберите элемент между датой и временем.

**Remarks**

[getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--) must be set before calling this method. If this method is called, [getSelectionLevel()](../../com.aspose.cells/timeline\#getSelectionLevel--) will be [getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | Дата и время начала |
| end | [DateTime](../../com.aspose.cells/datetime) | Дата и время окончания |
| вычислять | boolean | Указывает, следует ли вычислять относительные сводные таблицы |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Задает подпись этого Timeline.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


Текущий уровень времени Timeline.

Смотрите [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Возвращает или задает высоту указанного timeline в пикселях.

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


Возвращает или задает горизонтальное смещение формы timeline от её левого столбца в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Left. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Возвращает или задает имя указанного Timeline.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


Задает уровень времени, на котором была сделана текущая выборка для Timeline.

Смотрите [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


Указывает, следует ли отображать заголовок этого timeline.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


Указывает, следует ли отображать горизонтальную полосу прокрутки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


Указывает, следует ли отображать метку выбора.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


Указывает, следует ли отображать выпадающий список выбора уровня времени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Задает дату начала позиции прокрутки временного интервала этого [Timeline](../../com.aspose.cells/timeline).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Возвращает или задает вертикальное смещение формы timeline от её верхней строки в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Top. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Возвращает или задает ширину указанного timeline в пикселях.

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

