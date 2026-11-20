---
title: "Автофильтр"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет автофильтрацию для указанного листа."
type: docs
url: /ru/java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

Представляет автофильтрацию для указанного листа.

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | Добавляет фильтр по дате. |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | Добавляет фильтр по цвету заливки. |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | Добавляет фильтр для столбца фильтра. |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | Добавляет фильтр по цвету шрифта. |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | Добавляет фильтр по значку. |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | Фильтрует список с пользовательским критерием. |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | Фильтрует список с пользовательскими критериями. |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | Добавляет динамический фильтр. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | Фильтрует список с указанными критериями. |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | Отфильтровать топ‑10 элементов в списке |
| [getCellArea()](#getCellArea--) | Получает [CellArea](../../com.aspose.cells/cellarea), к которому применяется этот AutoFilter. |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | Получает [CellArea](../../com.aspose.cells/cellarea), к которому применяется указанный AutoFilter. |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | Получает коллекцию столбцов фильтра. |
| [getRange()](#getRange--) | Представляет диапазон, к которому применяется указанный AutoFilter. |
| [getShowFilterButton()](#getShowFilterButton--) | Указывает, видна ли кнопка AutoFilter для этого столбца. |
| [getSorter()](#getSorter--) | Получает сортировщик данных. |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | Соответствует всем пустым ячейкам в списке. |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | Соответствует всем непустым ячейкам в списке. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Обновить автофильтры, чтобы скрыть или показать строки. |
| [refresh(boolean hideRows)](#refresh-boolean-) | Получает индексы всех скрытых строк. |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | Удаляет фильтр по дате. |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | Удаляет конкретный фильтр. |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | Удаляет фильтр для столбца фильтра. |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | Устанавливает диапазон, к которому применяется указанный AutoFilter. |
| [setRange(String value)](#setRange-java.lang.String-) | Представляет диапазон, к которому применяется указанный AutoFilter. |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | Указывает, видна ли кнопка AutoFilter для этого столбца. |
| [showAll()](#showAll--) | Отобразить все строки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Добавляет фильтр по дате.

**Remarks**

Если DateTimeGroupingType имеет значение Year, влияет только параметр year. Если DateTiemGroupingType имеет значение Month, влияют только параметры year и month.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Тип группировки |
| год | int | Год. |
| месяц | int | Месяц. |
| день | int | День. |
| час | int | Час. |
| минута | int | Минута. |
| секунда | int | Секунда. |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


Добавляет фильтр по цвету заливки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Тип фонового узора. |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Цвет переднего плана. |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Цвет фона. |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


Добавляет фильтр для столбца фильтра.

**Remarks**

MS Excel 2007 поддерживает множественный выбор в столбце фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| критерий | java.lang.String | Указанный критерий (строка; например, "101"). Он может быть только null или одним из значений ячеек в этом столбце. |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


Добавляет фильтр по цвету шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | Объект [CellsColor](../../com.aspose.cells/cellscolor). |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


Добавляет фильтр по значку.

**Remarks**

Поддерживается только добавление фильтра значков. Не поддерживается проверка, какие строки видимы, если фильтр является фильтром значков.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype). Тип набора значков. |
| iconId | int | Идентификатор значка. |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


Фильтрует список с пользовательским критерием.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Тип оператора фильтра |
| criteria1 | java.lang.Object | Пользовательский критерий |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Фильтрует список с пользовательскими критериями.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Тип оператора фильтра |
| criteria1 | java.lang.Object | Пользовательский критерий |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Тип оператора фильтра |
| criteria2 | java.lang.Object | Пользовательский критерий |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


Добавляет динамический фильтр.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype). Тип динамического фильтра. |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


Фильтрует список с указанными критериями.

**Remarks**

Aspose.Cells удалит все остальные настройки фильтра в этом поле, как в MS Excel 97-2003.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| критерий | java.lang.String | Указанный критерий (строка; например, "101"). |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


Отфильтровать топ‑10 элементов в списке

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| isTop | boolean | Указывает, применяется ли фильтр сверху или снизу |
| isPercent | boolean | Указывает, является ли элемент процентом или количеством |
| itemCount | int | Количество элементов |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Получает [CellArea](../../com.aspose.cells/cellarea), к которому применяется этот AutoFilter.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


Получает [CellArea](../../com.aspose.cells/cellarea), к которому применяется указанный AutoFilter.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| refreshAppliedRange | boolean | Обновлять ли применённый диапазон. Для применённого диапазона автофильтра последняя строка может измениться при изменении данных ячеек. Если этот флаг установлен в true, последняя строка диапазона будет пересчитана в соответствии с текущими данными ячеек. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


Получает коллекцию столбцов фильтра.

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


Представляет диапазон, к которому применяется указанный AutoFilter.

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


Указывает, видна ли кнопка AutoFilter для этого столбца.

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


Получает сортировщик данных.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


Соответствует всем пустым ячейкам в списке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


Соответствует всем непустым ячейкам в списке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |

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
public int[] refresh()
```


Обновить автофильтры, чтобы скрыть или показать строки.

**Returns:**
int[] - Возвращает индексы всех скрытых строк.
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


Получает индексы всех скрытых строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| hideRows | boolean | Если true, скрыть отфильтрованные строки. |

**Returns:**
int[] - Возвращает индексы всех скрытых строк.
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Удаляет фильтр по дате.

**Remarks**

Если DateTimeGroupingType имеет значение Year, влияет только параметр year. Если DateTiemGroupingType имеет значение Month, влияют только параметры year и month.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Тип группировки |
| год | int | Год. |
| месяц | int | Месяц. |
| день | int | День. |
| час | int | Час. |
| минута | int | Минута. |
| секунда | int | Секунда. |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


Удаляет конкретный фильтр.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Конкретный индекс фильтра |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


Удаляет фильтр для столбца фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | Целочисленное смещение поля, на котором вы хотите основывать фильтр (слева от списка; самое левое поле имеет индекс 0). |
| критерий | java.lang.String | Указанный критерий (строка; например, "101"). Он может быть только null или одним из значений ячеек в этом столбце. |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


Устанавливает диапазон, к которому применяется указанный AutoFilter.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| startColumn | int | Индекс начального столбца. |
| endColumn | int | Индекс конечного столбца. |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


Представляет диапазон, к которому применяется указанный AutoFilter.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


Указывает, видна ли кнопка AutoFilter для этого столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


Отобразить все строки.

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

