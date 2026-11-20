---
title: "GridCell"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет объект ячейки."
type: docs
url: /ru/java/com.aspose.gridweb/gridcell/
---

**Inheritance:**
java.lang.Object
```
public class GridCell
```

Представляет объект ячейки.
## Методы

| Метод | Описание |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | Указывает, содержит ли эта ячейка внешнюю ссылку. |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | Копирует данные из исходной ячейки. |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | скопировать стиль и установить стиль для ячейки |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | Создает объект комментария для ячейки. |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | Создает объект проверки для ячейки. |
| [equals(Object obj)](#equals-java.lang.Object-) | Проверяет, ссылается ли этот объект на ту же ячейку, что и другой объект ячейки. |
| [getBoolValue()](#getBoolValue--) | Получает логическое значение, содержащееся в ячейке. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Получает номер столбца (нумерация с нуля) ячейки. |
| [getComment()](#getComment--) | Получить объект комментария в этой ячейке |
| [getDateValue()](#getDateValue--) | Получает значение DateTime, содержащееся в ячейке. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Получает отформатированное строковое значение этой ячейки. |
| [getDoubleValue()](#getDoubleValue--) | Получает значение double, содержащееся в ячейке. |
| [getFloatValue()](#getFloatValue--) | Получает значение float, содержащееся в ячейке. |
| [getFormula()](#getFormula--) | Получает формулу [GridCell](../../com.aspose.gridweb/gridcell). |
| [getHtmlString()](#getHtmlString--) | Получает HTML-строку, содержащую данные и некоторые форматирования в этой ячейке. |
| [getIntValue()](#getIntValue--) | Получает целочисленное значение, содержащееся в ячейке. |
| [getName()](#getName--) | Получает имя ячейки. |
| [getRow()](#getRow--) | Получает номер строки (нумерация с нуля) ячейки. |
| [getStringValue()](#getStringValue--) | Получает строковое значение, содержащееся в ячейке. |
| [getStyle()](#getStyle--) | Получает копию стиля ячейки. Установить стиль для ячейки. |
| [getType()](#getType--) | возвращает тип значения ячейки, значение можно посмотреть в GridCellValueType.java |
| [getValue()](#getValue--) | Получает значение, содержащееся в этой ячейке. |
| [getWidthOfValue()](#getWidthOfValue--) | Получает ширину значения в пикселях. |
| [hashCode()](#hashCode--) | Служит хеш-функцией для определённого типа. |
| [isErrorValue()](#isErrorValue--) | Проверяет, может ли формула правильно вычислить результат. |
| [isFormula()](#isFormula--) | Отображает, содержит ли указанная ячейка формулу. |
| [isStyleSet()](#isStyleSet--) | Указывает, установлен ли стиль ячейки. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | Помещает логическое значение в ячейку. |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | Помещает значение DateTime в ячейку. |
| [putValue(double param_double)](#putValue-double-) | Помещает значение double в ячейку. |
| [putValue(int param_int)](#putValue-int-) | Помещает целочисленное значение в ячейку. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Помещает объектное значение в ячейку. то же, что setValue(Object param\_object) |
| [putValue(String param_string)](#putValue-java.lang.String-) | Помещает строковое значение в ячейку. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Помещает строковое значение в ячейку и при необходимости преобразует его в другой тип данных. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Помещает значение в ячейку; при необходимости значение будет преобразовано к другому типу данных, а числовой формат ячейки будет сброшен. |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | Устанавливает значение ячейки строковым значением и задает формат ячейки в соответствии с этим значением. |
| [removeComment()](#removeComment--) | Удаляет объект комментария ячейки. |
| [removeValidation()](#removeValidation--) | Удаляет объект проверки ячейки. |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | Устанавливает границы (верх, низ, слева и справа) для ячейки, все границы имеют одинаковый стиль. |
| [setCustom(String custom)](#setCustom-java.lang.String-) | устанавливает пользовательский формат, null или пустая строка означают отсутствие пользовательского формата. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Устанавливает формулу [GridCell](../../com.aspose.gridweb/gridcell). |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Установить формулу и значение формулы. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Устанавливает HTML-строку, содержащую данные и некоторые форматирования в этой ячейке. |
| [setNumberType(int numbertype)](#setNumberType-int-) | установить формат отображения чисел и дат |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Получает копию стиля ячейки. Установить стиль для ячейки. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Получает значение, содержащееся в этой ячейке. |
| [toString()](#toString--) | Возвращает строку, представляющую текущий объект Cell. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только когда ячейка является формульной.

**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```


Копирует данные из исходной ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | Исходный объект [GridCell](../../com.aspose.gridweb/gridcell). |

### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```


скопировать стиль и установить стиль для ячейки

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Исходный стиль. |

### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```


Создает объект комментария для ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| примечание | java.lang.String | примечание к комментарию. |
| автор | java.lang.String | автор комментария. |
| isvisible | boolean | является ли комментарий видимым. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```


Создает объект проверки для ячейки.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
         		// Sets to number validation expression.
         		v.setRegEx("\\d+");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype). Тип проверки. |
| isRequried | boolean | Требуется ли значение ячейки. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - 
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Проверяет, ссылается ли этот объект на ту же ячейку, что и другой объект ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | другой объект GridCell |

**Returns:**
логический - true, если два объекта ячейки ссылаются на одну и ту же ячейку.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Получает логическое значение, содержащееся в ячейке.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Получает номер столбца (нумерация с нуля) ячейки.

**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```


Получить объект комментария в этой ячейке

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```


Получает значение DateTime, содержащееся в ячейке.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Получает отформатированное строковое значение этой ячейки.

**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Получает значение double, содержащееся в ячейке.

**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Получает значение float, содержащееся в ячейке.

**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```


Получает формулу [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Строка формулы всегда начинается со знака равенства (=). И, пожалуйста, всегда используйте запятую (,) в качестве разделителя параметров, например "=SUM(A1, E1, H2)".

Пользователь может задать любую формулу в файле дизайнера Workbook. Aspose.Cells сохранит все формулы. Если пользователь использует это свойство для установки формулы в ячейку, поддерживается большая часть встроенных функций Workbook. И будет добавлено больше. Если у вас есть особые потребности в встроенных функциях Workbook, пожалуйста, дайте нам знать.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         sheet.getCells().get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Получает HTML-строку, содержащую данные и некоторые форматирования в этой ячейке.

**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Получает целочисленное значение, содержащееся в ячейке.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Получает имя ячейки. Например: A1, F102.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Получает номер строки (нумерация с нуля) ячейки.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Получает строковое значение, содержащееся в ячейке.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Получает копию стиля ячейки. Установить стиль для ячейки.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```


возвращает тип значения ячейки, значение можно посмотреть в GridCellValueType.java

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Получает значение, содержащееся в этой ячейке.

**Remarks**

Возможный тип:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Получает ширину значения в пикселях.

**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```


Служит хеш-функцией для определённого типа.

**Returns:**
int — хеш‑код текущего объекта GridCell.
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Проверяет, может ли формула правильно вычислить результат.

**Remarks**

Применяется только к ячейке с формулой.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Отображает, содержит ли указанная ячейка формулу.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Указывает, установлен ли стиль ячейки. Если возвращается false, это означает, что у ячейки используется формат по умолчанию.

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




### putValue(boolean param_boolean) {#putValue-boolean-}
```
public void putValue(boolean param_boolean)
```


Помещает логическое значение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| param_boolean | boolean | Входное значение |

### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```


Помещает значение DateTime в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | Входное значение |

### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```


Помещает значение double в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| param_double | double | Входное значение |

### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```


Помещает целочисленное значение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| param_int | int | Входное значение |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Помещает объектное значение в ячейку. то же, что setValue(Object param\_object)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| objectValue | java.lang.Object | входное значение |

### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```


Помещает строковое значение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| param_string | java.lang.String | Входное значение |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Помещает строковое значение в ячейку и при необходимости преобразует его в другой тип данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | java.lang.String | Входное значение |
| isConverted | boolean | True: преобразовано в другой тип данных, если это уместно. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Помещает значение в ячейку; при необходимости значение будет преобразовано к другому типу данных, а числовой формат ячейки будет сброшен.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | java.lang.String | Входное значение |
| isConverted | boolean | True: преобразовано в другой тип данных, если это уместно. |
| setStyle | boolean | True: установить числовой формат в стиль ячейки при преобразовании в другой тип данных |

### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```


Устанавливает значение ячейки строковым значением и задает формат ячейки в соответствии с этим значением.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | java.lang.String | Входное значение. |

### removeComment() {#removeComment--}
```
public void removeComment()
```


Удаляет объект комментария ячейки.

### removeValidation() {#removeValidation--}
```
public void removeValidation()
```


Удаляет объект проверки ячейки.

### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```


Устанавливает границы (верх, низ, слева и справа) для ячейки, все границы имеют одинаковый стиль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Стиль границы. |

### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```


устанавливает пользовательский формат, null или пустая строка означают отсутствие пользовательского формата.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пользовательский | java.lang.String | пользовательское строковое представление |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Устанавливает формулу [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Строка формулы всегда начинается со знака равенства (=). И, пожалуйста, всегда используйте запятую (,) в качестве разделителя параметров, например "=SUM(A1, E1, H2)".

Пользователь может задать любую формулу в файле дизайнера Workbook. Aspose.Cells сохранит все формулы. Если пользователь использует это свойство для установки формулы в ячейку, поддерживается большая часть встроенных функций Workbook. И будет добавлено больше. Если у вас есть особые потребности в встроенных функциях Workbook, пожалуйста, дайте нам знать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Установить формулу и значение формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула. |
| значение | java.lang.Object | Значение формулы. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Устанавливает HTML-строку, содержащую данные и некоторые форматирования в этой ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```


установить формат отображения чисел и дат

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| numbertype | int | значение numbertype, см. GridTableItemStyle.NumberType |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Получает копию стиля ячейки. Установить стиль для ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Получает значение, содержащееся в этой ячейке.

**Remarks**

Возможный тип:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```


Возвращает строку, представляющую текущий объект Cell.

**Returns:**
java.lang.String -
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

