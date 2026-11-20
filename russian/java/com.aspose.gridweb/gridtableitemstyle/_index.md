---
title: "GridTableItemStyle"
second_title: "Справочник API Aspose.Cells for Java"
description: "Наследуется от System.Web.UI.WebControls.TableItemStyle."
type: docs
url: /ru/java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```

Наследуется от System.Web.UI.WebControls.TableItemStyle. Инкапсулирует стили WebCell.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheetCollection sheets = GridWeb1.getWorkSheets();
 
         GridWorksheet sheet = sheets.add("demo1");
 
         sheet.getCells().get(0,0).putValue("Demo Text");
         GridTableItemStyle style = sheet.getCells().get(0, 0).getStyle();
 
         style.getFont().setSize(FontUnit.Point(72));
         style.setWrap(false);
 
         style.setBackColor(Color.getGray());
         	style.setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.setBorderWidth(Unit.Pixel(1));
         style.setBorderColor(Color.getSilver());
         style.getRightBorderStyle().setBorderColor(Color.getBlack());
         	style.getRightBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         	style.getRightBorderStyle().setBorderWidth(Unit.Pixel(1));
         style.getBottomBorderStyle().setBorderColor(Color.getBlack());
         style.getBottomBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.getBottomBorderStyle().setBorderWidth(Unit.Pixel(1));
         sheet.getCells().get(0, 0).setStyle(style);
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | Конструктор по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | Копирует из другого объекта стиля. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Получает BackColor в стиле |
| [getBackImageAttributes()](#getBackImageAttributes--) | Атрибуты фонового изображения. |
| [getBackImageUrl()](#getBackImageUrl--) | URL фонового изображения. |
| [getBorderColor()](#getBorderColor--) | Получает BorderColor в стиле |
| [getBorderStyle()](#getBorderStyle--) | Получает BorderStyle в стиле |
| [getBorderWidth()](#getBorderWidth--) | Получает BorderWidth в стиле |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | Указывает стиль нижней границы ячейки. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Получает CssClass в стиле |
| [getCustom()](#getCustom--) | Получает пользовательский формат, null или пустая строка означают отсутствие пользовательского формата. |
| [getFont()](#getFont--) | Получает Font в стиле |
| [getForeColor()](#getForeColor--) | Получает ForeColor в стиле |
| [getHeight()](#getHeight--) | Получает Height в стиле |
| [getHorizontalAlign()](#getHorizontalAlign--) | Получает HorizontalAlign в стиле |
| [getIndentLevel()](#getIndentLevel--) | Получает уровень отступа. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | Указывает стиль левой границы ячейки. |
| [getNumberType()](#getNumberType--) | Получает формат отображения чисел и дат. |
| [getQuotePrefix()](#getQuotePrefix--) | Указывает, начинается ли значение ячейки с одинарной кавычки. |
| [getRightBorderStyle()](#getRightBorderStyle--) | Указывает стиль правой границы ячейки. |
| [getRotationAngle()](#getRotationAngle--) | Получает атрибут Rotation. |
| [getTopBorderStyle()](#getTopBorderStyle--) | Указывает стиль верхней границы ячейки. |
| [getVerticalAlign()](#getVerticalAlign--) | Получает значение VerticalAlign в стиле. |
| [getWidth()](#getWidth--) | Получает Width в стиле |
| [getWrap()](#getWrap--) | Получает значение Wrap в стиле. |
| [hashCode()](#hashCode--) | Служит хеш-функцией для конкретного типа, подходящей для использования в хеш-алгоритмах и структурах данных, таких как хеш-таблица. |
| [isLocked()](#isLocked--) | Получает значение, указывающее, может ли ячейка быть изменена, когда её лист защищён. |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | Объединяется с другим объектом стиля. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Устанавливает BackColor в стиле |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | Атрибуты фонового изображения. |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | URL фонового изображения. |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Устанавливает BorderColor в стиле |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Устанавливает BorderStyle в стиле |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Устанавливает BorderWidth в стиле |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Указывает стиль нижней границы ячейки. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Устанавливает CssClass в стиле |
| [setCustom(String value)](#setCustom-java.lang.String-) | Устанавливает пользовательский формат, null или пустая строка означают отсутствие пользовательского формата. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Устанавливает ForeColor в стиле |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Устанавливает Height в стиле |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | Устанавливает HorizontalAlign в стиле |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Устанавливает уровень отступа. |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Указывает стиль левой границы ячейки. |
| [setLocked(boolean value)](#setLocked-boolean-) | Устанавливает значение, указывающее, может ли ячейка быть изменена, когда её лист защищён. |
| [setNumberType(int value)](#setNumberType-int-) | Устанавливает формат отображения чисел и дат. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Указывает, начинается ли значение ячейки с одинарной кавычки. |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Указывает стиль правой границы ячейки. |
| [setRotationAngle(short value)](#setRotationAngle-short-) | Устанавливает атрибут Rotation. |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Указывает стиль верхней границы ячейки. |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | Устанавливает значение VerticalAlign в стиле. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Устанавливает Width в стиле |
| [setWrap(boolean value)](#setWrap-boolean-) | Устанавливает значение Wrap в стиле. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```


Конструктор по умолчанию.

### copyFrom(WebStyle s) {#copyFrom-com.aspose.gridweb.WebStyle-}
```
public void copyFrom(WebStyle s)
```


Копирует из другого объекта стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | другой объект стиля |

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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Получает BackColor в стиле

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```


Атрибуты фонового изображения.

**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```


URL фонового изображения.

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Получает BorderColor в стиле

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Получает BorderStyle в стиле

Смотрите [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Получает BorderWidth в стиле

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```


Указывает стиль нижней границы ячейки.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


Получает CssClass в стиле

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Получает пользовательский формат, null или пустая строка означают отсутствие пользовательского формата.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Получает Font в стиле

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Получает ForeColor в стиле

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Получает Height в стиле

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```


Получает HorizontalAlign в стиле

Смотрите [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Получает уровень отступа.

**Remarks**

**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```


Указывает стиль левой границы ячейки.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Возвращает формат отображения чисел и дат. Шаблоны форматирования различаются в разных регионах.

**Remarks**

Например, шаблоны форматирования, представленные цифрами, для региона en\_US:

| Значение | Тип | Строка формата |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Красный](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Красный](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ДП/ПП` |
| 19 | Time | `h:mm:ss ДП/ПП` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Красный](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Красный](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Указывает, начинается ли значение ячейки с одинарной кавычки.

**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```


Указывает стиль правой границы ячейки.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```


Получает атрибут Rotation.

**Remarks**

0: Не повернут.

255: Сверху вниз.

\-90: Вниз.

90: Вверх.

Вы можете установить 255 или значение в диапазоне от -90 до 90.

**Returns:**
short
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```


Указывает стиль верхней границы ячейки.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```


Получает значение VerticalAlign в стиле.

Смотрите [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Получает Width в стиле

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```


Получает значение Wrap в стиле.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Служит хеш-функцией для конкретного типа, подходящей для использования в хеш-алгоритмах и структурах данных, таких как хеш-таблица.

**Returns:**
int - Хеш-код для текущего стиля.
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Получает значение, указывающее, может ли ячейка быть изменена, когда лист защищён. Когда лист защищён и IsLocked равно true, ячейка не может быть отредактирована. Когда лист защищён и IsLocked равно false, ячейка может быть отредактирована.

**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```


Объединяется с другим объектом стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | другой объект стиля |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Устанавливает BackColor в стиле

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


Атрибуты фонового изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


URL фонового изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Устанавливает BorderColor в стиле

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Устанавливает BorderStyle в стиле

Смотрите [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Устанавливает BorderWidth в стиле

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


Указывает стиль нижней границы ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Устанавливает CssClass в стиле

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Устанавливает пользовательский формат, null или пустая строка означают отсутствие пользовательского формата.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Устанавливает ForeColor в стиле

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Устанавливает Height в стиле

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```


Устанавливает HorizontalAlign в стиле

Смотрите [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Устанавливает уровень отступа.

**Remarks**

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


Указывает стиль левой границы ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Устанавливает значение, указывающее, может ли ячейка быть изменена, когда лист защищён. Когда лист защищён и IsLocked равно true, ячейка не может быть отредактирована. Когда лист защищён и IsLocked равно false, ячейка может быть отредактирована.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Устанавливает формат отображения чисел и дат. Шаблоны форматирования различаются для разных регионов.

**Remarks**

Например, шаблоны форматирования, представленные цифрами, для региона en\_US:

| Значение | Тип | Строка формата |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Красный](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Красный](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ДП/ПП` |
| 19 | Time | `h:mm:ss ДП/ПП` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Красный](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Красный](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Указывает, начинается ли значение ячейки с одинарной кавычки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


Указывает стиль правой границы ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


Устанавливает атрибут Rotation.

**Remarks**

0: Не повернут.

255: Сверху вниз.

\-90: Вниз.

90: Вверх.

Вы можете установить 255 или значение в диапазоне от -90 до 90.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | short |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


Указывает стиль верхней границы ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```


Устанавливает значение VerticalAlign в стиле.

Смотрите [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Устанавливает Width в стиле

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```


Устанавливает значение Wrap в стиле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

