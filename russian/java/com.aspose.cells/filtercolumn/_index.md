---
title: "FilterColumn"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет фильтр для отдельного столбца или столбца в таблице."
type: docs
url: /ru/java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

Представляет фильтр для отдельного столбца или столбца в таблице.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | Получает [ColorFilter](../../com.aspose.cells/colorfilter) для фильтрации данных по цвету. |
| [getCustomFilters()](#getCustomFilters--) | Получает [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) для фильтрации данных по пользовательским критериям. |
| [getDynamicFilter()](#getDynamicFilter--) | Получает [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) для фильтрации с динамическими критериями. |
| [getFieldIndex()](#getFieldIndex--) | Получает смещение столбца в диапазоне. |
| [getFilter()](#getFilter--) | Получает условие фильтрации данных. |
| [getFilterType()](#getFilterType--) | Получает тип фильтрации данных. |
| [getFilterValues()](#getFilterValues--) | Получает [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) для фильтрации данных по меткам или дате и времени. |
| [getIconFilter()](#getIconFilter--) | Получает [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) для фильтрации данных по значку. |
| [getMultipleFilters()](#getMultipleFilters--) | Получает [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) для фильтрации данных по меткам или дате и времени. |
| [getTop10Filter()](#getTop10Filter--) | Получает [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) для фильтрации данных по рангу. |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | Указывает, видна ли кнопка AutoFilter для этого столбца. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | Выбирает всё. |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | Получает [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) для фильтрации данных по пользовательским критериям. |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | Указывает, видна ли кнопка AutoFilter для этого столбца. |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Устанавливает смещение столбца в диапазоне. |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | Устанавливает условие фильтрации данных. |
| [setFilterType(int value)](#setFilterType-int-) | Устанавливает тип фильтрации данных. |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | Получает [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) для фильтрации данных по меткам или дате и времени. |
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
### getColorFilter() {#getColorFilter--}
```
public ColorFilter getColorFilter()
```


Получает [ColorFilter](../../com.aspose.cells/colorfilter) для фильтрации данных по цвету.

**Remarks**

Устанавливает [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) как [FilterType.COLOR\_FILTER](../../com.aspose.cells/filtertype\#COLOR-FILTER) первым, иначе будет возвращён Null.

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


Получает [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) для фильтрации данных по пользовательским критериям.

**Remarks**

ПРИМЕЧАНИЕ: Этот сеттер свойства теперь устарел. Вместо этого используйте свойство [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) задавая его как [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Это свойство будет удалено через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


Получает [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) для фильтрации с динамическими критериями.

**Remarks**

Перед использованием этого свойства убедитесь, что [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) имеет значение [FilterType.DYNAMIC\_FILTER](../../com.aspose.cells/filtertype\#DYNAMIC-FILTER), иначе будет возвращён null.

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Получает смещение столбца в диапазоне.

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


Получает условие фильтрации данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого используйте соответствующее свойство в соответствии с [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). И для типа фильтра [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) возвращаемый объект теперь является [FilterValueCollection](../../com.aspose.cells/filtervaluecollection), а не [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Это свойство будет удалено через 12 месяцев, начиная с октября 2025 года. Aspise приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Получает тип фильтрации данных.

Смотрите [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

Соответствующий объект фильтра будет создан, когда это свойство установлено, и соответствующее свойство следует использовать для получения объекта фильтра соответственно:

| FilterType | Свойство |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Returns:**
int
### getFilterValues() {#getFilterValues--}
```
public FilterValueCollection getFilterValues()
```


Получает [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) для фильтрации данных по меткам или дате и времени.

**Remarks**

Устанавливает [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) как [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) сначала, иначе будет возвращён Null.

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


Получает [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) для фильтрации данных по значку.

**Remarks**

Перед использованием этого свойства, пожалуйста, убедитесь, что [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) является [FilterType.ICON\_FILTER](../../com.aspose.cells/filtertype\#ICON-FILTER), иначе будет возвращён null.

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


Получает [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) для фильтрации данных по меткам или дате и времени.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство FilterColumn.FilterValues. Это свойство будет удалено через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


Получает [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) для фильтрации данных по рангу.

**Remarks**

Перед использованием этого свойства, пожалуйста, убедитесь, что [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) является [FilterType.TOP\_10](../../com.aspose.cells/filtertype\#TOP-10), иначе будет возвращён null.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDropdownVisible() {#isDropdownVisible--}
```
public boolean isDropdownVisible()
```


Указывает, видна ли кнопка AutoFilter для этого столбца.

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




### selectAll() {#selectAll--}
```
public void selectAll()
```


Выбирает всё.

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


Получает [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) для фильтрации данных по пользовательским критериям.

**Remarks**

ПРИМЕЧАНИЕ: Этот сеттер свойства теперь устарел. Вместо этого используйте свойство [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) задавая его как [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Это свойство будет удалено через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


Указывает, видна ли кнопка AutoFilter для этого столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Устанавливает смещение столбца в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


Устанавливает условие фильтрации данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого используйте соответствующее свойство в соответствии с [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). И для типа фильтра [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) возвращаемый объект теперь является [FilterValueCollection](../../com.aspose.cells/filtervaluecollection), а не [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Это свойство будет удалено через 12 месяцев, начиная с октября 2025 года. Aspise приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


Устанавливает тип фильтрации данных.

Смотрите [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

Соответствующий объект фильтра будет создан, когда это свойство установлено, и соответствующее свойство следует использовать для получения объекта фильтра соответственно:

| FilterType | Свойство |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


Получает [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) для фильтрации данных по меткам или дате и времени.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство FilterColumn.FilterValues. Это свойство будет удалено через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) |  |

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

