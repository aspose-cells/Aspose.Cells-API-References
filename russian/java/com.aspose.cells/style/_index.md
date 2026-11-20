---
title: "Style"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет стиль отображения Excel‑документа, например шрифт, цвет, выравнивание, границу и т.д."
type: docs
url: /ru/java/com.aspose.cells/style/
---

**Inheritance:**
java.lang.Object
```
public class Style
```

Представляет стиль отображения Excel‑документа, например шрифт, цвет, выравнивание, границу и т.д. Объект Style содержит все атрибуты стиля (шрифт, числовой формат, выравнивание и т.п.) в виде свойств.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
         Style style =  cell.getStyle();
         style.getFont().setName("Times New Roman");
         style.getFont().setColor(Color.getBlue());
         cell.setStyle(style);
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Style()](#Style--) | Инициализирует новый экземпляр класса [Style](../../com.aspose.cells/style). |
## Методы

| Метод | Описание |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | Копирует данные из другого объекта стиля |
| [equals(Object obj)](#equals-java.lang.Object-) | Определяет, равны ли два экземпляра Style. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | Получает цвет фона в виде 32‑битного значения ARGB. |
| [getBackgroundColor()](#getBackgroundColor--) | Получает цвет фона стиля. |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | Получает цвет темы фона. |
| [getBorders()](#getBorders--) | Получает [BorderCollection](../../com.aspose.cells/bordercollection) стиля. |
| [getBottomBorder()](#getBottomBorder--) | Получает нижнюю границу. |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | Получает строку шаблона, зависящую от культуры, для числового формата. |
| [getCustom()](#getCustom--) | Представляет строку пользовательского числового формата этого объекта стиля. |
| [getFont()](#getFont--) | Получает объект [getFont()](../../com.aspose.cells/style\#getFont--). |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | Получает цвет переднего плана в виде 32‑битного значения ARGB. |
| [getForegroundColor()](#getForegroundColor--) | Получает цвет переднего плана стиля. |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | Получает цвет переднего плана темы. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Получает тип горизонтального выравнивания текста в ячейке. |
| [getIndentLevel()](#getIndentLevel--) | Представляет уровень отступа для ячейки или диапазона. |
| [getInvariantCustom()](#getInvariantCustom--) | Получает независимую от культуры строку шаблона для числового формата. |
| [getLeftBorder()](#getLeftBorder--) | Получает левую границу. |
| [getName()](#getName--) | Получает название стиля. |
| [getNumber()](#getNumber--) | Получает формат отображения чисел и дат. |
| [getParentStyle()](#getParentStyle--) | Получает родительский стиль этого стиля. |
| [getPattern()](#getPattern--) | Получает тип шаблона фона ячейки. |
| [getQuotePrefix()](#getQuotePrefix--) | Указывает, начинается ли значение ячейки с одинарной кавычки. |
| [getRightBorder()](#getRightBorder--) | Получает правую границу. |
| [getRotationAngle()](#getRotationAngle--) | Представляет угол поворота текста. |
| [getShrinkToFit()](#getShrinkToFit--) | Представляет, автоматически ли текст уменьшается, чтобы поместиться в доступную ширину столбца. |
| [getTextDirection()](#getTextDirection--) | Представляет порядок чтения текста. |
| [getTopBorder()](#getTopBorder--) | Получает верхнюю границу. |
| [getTwoColorGradient()](#getTwoColorGradient--) | Получает настройку двухцветного градиента. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | Получает настройку двухцветного градиента. |
| [getVerticalAlignment()](#getVerticalAlignment--) | Получает тип вертикального выравнивания текста в ячейке. |
| [hasBorders()](#hasBorders--) | Проверяет, были ли установлены границы для стиля. |
| [hashCode()](#hashCode--) | Служит хеш-функцией для объекта Style. |
| [isAlignmentApplied()](#isAlignmentApplied--) | Указывает, следует ли применять форматирование выравнивания. |
| [isBorderApplied()](#isBorderApplied--) | Указывает, следует ли применять форматирование границы. |
| [isCheckBox()](#isCheckBox--) | Указывает, является ли это стилем флажка. |
| [isDateTime()](#isDateTime--) | Указывает, является ли числовой формат датой. |
| [isFillApplied()](#isFillApplied--) | Указывает, следует ли применять форматирование заливки. |
| [isFontApplied()](#isFontApplied--) | Указывает, следует ли применять форматирование шрифта. |
| [isFormulaHidden()](#isFormulaHidden--) | Представляет, будет ли формула скрыта, когда лист защищён. |
| [isGradient()](#isGradient--) | Указывает, является ли затенение ячейки градиентным шаблоном. |
| [isJustifyDistributed()](#isJustifyDistributed--) | Указывает, следует ли использовать выравнивание ячеек по ширине или распределённое выравнивание в последней строке текста. |
| [isLocked()](#isLocked--) | Получает значение, указывающее, может ли ячейка быть изменена или нет. |
| [isModified(int modifyFlag)](#isModified-int-) | Проверяет, были ли изменены указанные свойства стиля. |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | Указывает, следует ли применять форматирование чисел. |
| [isPercent()](#isPercent--) | Указывает, является ли числовой формат процентным. |
| [isProtectionApplied()](#isProtectionApplied--) | Указывает, следует ли применять форматирование защиты. |
| [isTextWrapped()](#isTextWrapped--) | Получает значение, указывающее, перенесён ли текст внутри ячейки. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | Указывает, следует ли применять форматирование выравнивания. |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | Устанавливает цвет фона с помощью 32-битного значения ARGB. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Устанавливает цвет фона стиля. |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | Устанавливает цвет фоновой темы. |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | Устанавливает границы стиля. |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | Устанавливает границы стиля. |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | Указывает, следует ли применять форматирование границы. |
| [setCheckBox(boolean value)](#setCheckBox-boolean-) | Указывает, является ли это стилем флажка. |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | Устанавливает зависящую от культуры строку шаблона для числового формата. |
| [setCustom(String value)](#setCustom-java.lang.String-) | Представляет строку пользовательского числового формата этого объекта стиля. |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | Устанавливает пользовательскую строку числового формата ячейки. |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | Указывает, следует ли применять форматирование заливки. |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | Указывает, следует ли применять форматирование шрифта. |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | Устанавливает цвет переднего плана с помощью 32-битного значения ARGB. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Устанавливает цвет переднего плана стиля. |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | Устанавливает цвет темы переднего плана. |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | Представляет, будет ли формула скрыта, когда лист защищён. |
| [setGradient(boolean value)](#setGradient-boolean-) | Указывает, является ли затенение ячейки градиентным шаблоном. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Устанавливает тип горизонтального выравнивания текста в ячейке. |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Представляет уровень отступа для ячейки или диапазона. |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | Указывает, следует ли использовать выравнивание ячеек по ширине или распределённое выравнивание в последней строке текста. |
| [setLocked(boolean value)](#setLocked-boolean-) | Устанавливает значение, указывающее, может ли ячейка быть изменена или нет. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя стиля. |
| [setNumber(int value)](#setNumber-int-) | Устанавливает формат отображения чисел и дат. |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | Указывает, следует ли применять форматирование чисел. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Установите контурные границы |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Установите контурные границы |
| [setPattern(int value)](#setPattern-int-) | Устанавливает тип шаблона фона ячейки. |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | Устанавливает цвет фона. |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | Указывает, следует ли применять форматирование защиты. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Указывает, начинается ли значение ячейки с одинарной кавычки. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Представляет угол поворота текста. |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | Представляет, автоматически ли текст уменьшается, чтобы поместиться в доступную ширину столбца. |
| [setTextDirection(int value)](#setTextDirection-int-) | Представляет порядок чтения текста. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Устанавливает значение, указывающее, перенесён ли текст внутри ячейки. |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Устанавливает указанную заливку в двухцветный градиент. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Устанавливает тип вертикального выравнивания текста в ячейке. |
| [toJson()](#toJson--) | Преобразовать [Style](../../com.aspose.cells/style) в данные JSON‑структуры. |
| [toString()](#toString--) |  |
| [update()](#update--) | Применить именованный стиль к стилям ячеек, использующим этот именованный стиль. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```


Инициализирует новый экземпляр класса [Style](../../com.aspose.cells/style).

**Remarks**

ПРИМЕЧАНИЕ: Этот конструктор теперь устарел. Вместо него, пожалуйста, используйте метод CellsFactory.CreateStyle(). Это свойство будет удалено через 6 месяцев, начиная с октября 2016 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```


Копирует данные из другого объекта стиля

**Remarks**

Этот метод не копирует имя стиля. Если вы хотите скопировать имя, пожалуйста, вызовите следующий код после копирования стиля: destStyle.Name = style.Name.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Исходный объект Style |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Определяет, равны ли два экземпляра Style.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | Объект Style для сравнения с текущим объектом Style. |

**Returns:**
boolean — true, если указанный объект равен текущему объекту; иначе false.
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```


Получает цвет фона в виде 32‑битного значения ARGB.

**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Получает цвет фона стиля.

**Remarks**

Если вы хотите задать цвет ячейки, используйте свойство Style.ForegroundColor. Это свойство будет применено только если шаблон стиля ячейки отличается от none или solid.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```


Получает цвет темы фона.

**Remarks**

Если цвет фона не является цветом темы, будет возвращено NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```


Получает [BorderCollection](../../com.aspose.cells/bordercollection) стиля.

**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
### getBottomBorder() {#getBottomBorder--}
```
public Border getBottomBorder()
```


Получает нижнюю границу.

**Returns:**
[Border](../../com.aspose.cells/border)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCultureCustom() {#getCultureCustom--}
```
public String getCultureCustom()
```


Возвращает строку шаблона формата числа, зависящую от культуры. Если для этого объекта не установлен формат числа, будет возвращено null. Если формат числа встроенный, будет возвращена строка шаблона, соответствующая встроенному формату.

**Remarks**

Для встроенного формата числа как содержимое шаблона (например, один встроенный формат даты — "m/d/y" для некоторых локалей, а для других локалей он становится "d/m/y"), так и спецификатор формата (например, некоторые локали используют символ, отличный от 'y', для обозначения части года в формате даты) зависят от культуры; для пользовательского пользовательского формата только спецификаторы формата изменяются в соответствии с культурой, остальные части шаблона форматирования не изменяются.

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Представляет строку пользовательского числового формата этого объекта стиля. Если пользовательский числовой формат не установлен (например, формат числа встроенный), будет возвращена пустая строка "".

**Remarks**

Возвращаемая пользовательская строка не зависит от культуры.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


Получает объект [getFont()](../../com.aspose.cells/style\#getFont--).

**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```


Получает цвет переднего плана в виде 32‑битного значения ARGB.

**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Получает цвет переднего плана стиля.

**Remarks**

Это означает отсутствие настройки цвета, если возвращено Color.Empty.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```


Получает цвет переднего плана темы.

**Remarks**

Если цвет переднего плана не является цветом темы, будет возвращено NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Получает тип горизонтального выравнивания текста в ячейке.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Представляет уровень отступа для ячейки или диапазона. Может быть только целым числом от 0 до 250.

**Remarks**

Если тип горизонтального выравнивания текста установлен в значение, отличное от left или right, уровень отступа будет сброшен до нуля.

**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```


Возвращает строку шаблона формата числа, не зависящую от культуры. Если для этого объекта не установлен формат числа, будет возвращено null. Если формат числа встроенный, будет возвращена строка шаблона, соответствующая встроенному формату.

**Remarks**

Для встроенных числовых форматов возвращаемое содержимое шаблона всё ещё зависит от культуры, например, для некоторых локалей оно возвращает "m/d/y", а для других локалей — "d/m/y". Отличие от [getCultureCustom()](../../com.aspose.cells/style\#getCultureCustom--) заключается (это также то, что означает независимость от культуры): спецификаторы формата и разделители сохраняются в стандартном виде, например, '/' всегда будет использоваться как разделитель даты и времени, а "y" всегда будет использоваться как часть "год", независимо от того, какой другой специальный символ используется для конкретной локали.

**Returns:**
java.lang.String
### getLeftBorder() {#getLeftBorder--}
```
public Border getLeftBorder()
```


Получает левую границу.

**Returns:**
[Border](../../com.aspose.cells/border)
### getName() {#getName--}
```
public String getName()
```


Получает название стиля.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
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
### getParentStyle() {#getParentStyle--}
```
public Style getParentStyle()
```


Получает родительский стиль этого стиля.

**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```


Получает тип шаблона фона ячейки.

Смотрите [BackgroundType](../../com.aspose.cells/backgroundtype).

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Указывает, начинается ли значение ячейки с одинарной кавычки.

**Returns:**
boolean
### getRightBorder() {#getRightBorder--}
```
public Border getRightBorder()
```


Получает правую границу.

**Returns:**
[Border](../../com.aspose.cells/border)
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Представляет угол поворота текста.

**Remarks**

0: Не повернут.

255: Сверху вниз.

\-90: Вниз.

90: Вверх.

Вы можете установить 255 или значение в диапазоне от -90 до 90.

**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```


Представляет, автоматически ли текст уменьшается, чтобы поместиться в доступную ширину столбца.

**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Представляет порядок чтения текста.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getTopBorder() {#getTopBorder--}
```
public Border getTopBorder()
```


Получает верхнюю границу.

**Returns:**
[Border](../../com.aspose.cells/border)
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```


Получает настройку двухцветного градиента.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Style.GetTwoColorGradientSetting() . Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.Object[] - Возвращает все настройки двухцветного градиента [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```


Получает настройку двухцветного градиента.

**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Получает тип вертикального выравнивания текста в ячейке.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```


Проверяет, были ли установлены границы для стиля.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Служит хеш-функцией для объекта Style.

**Remarks**

Этот метод предназначен только для внутреннего использования.

**Returns:**
int - Хеш‑код текущего объекта.
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```


Указывает, следует ли применять форматирование выравнивания.

**Remarks**

Только для именованного стиля.

**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```


Указывает, следует ли применять форматирование границы.

**Remarks**

Только для именованного стиля.

**Returns:**
boolean
### isCheckBox() {#isCheckBox--}
```
public boolean isCheckBox()
```


Указывает, является ли это стилем флажка.

**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```


Указывает, является ли числовой формат датой.

**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```


Указывает, следует ли применять форматирование заливки.

**Remarks**

Только для именованного стиля.

**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```


Указывает, следует ли применять форматирование шрифта.

**Remarks**

Только для именованного стиля.

**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```


Представляет, будет ли формула скрыта, когда лист защищён.

**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```


Указывает, является ли затенение ячейки градиентным шаблоном.

**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```


Указывает, следует ли использовать выравнивание ячеек по ширине или распределённое выравнивание в последней строке текста.

**Remarks**

Это типично для восточноазиатского выравнивания, но не типично в других контекстах. Работает только при распределённом горизонтальном выравнивании.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Получает значение, указывающее, может ли ячейка быть изменена или нет.

**Remarks**

Блокировка ячеек не оказывает эффекта, если лист не защищён.

**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```


Проверяет, были ли изменены указанные свойства стиля. Используется для стиля условного форматирования, чтобы проверить, следует ли использовать указанные свойства этого стиля при применении условного форматирования к ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). Флаги изменённого стиля |

**Returns:**
boolean - true, если указанные свойства были изменены
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```


Указывает, следует ли применять форматирование чисел.

**Remarks**

Только для именованного стиля.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Указывает, является ли числовой формат процентным.

**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```


Указывает, следует ли применять форматирование защиты.

**Remarks**

Только для именованного стиля.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Получает значение, указывающее, перенесён ли текст внутри ячейки.

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




### setAlignmentApplied(boolean value) {#setAlignmentApplied-boolean-}
```
public void setAlignmentApplied(boolean value)
```


Указывает, следует ли применять форматирование выравнивания.

**Remarks**

Только для именованного стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```


Устанавливает цвет фона с помощью 32-битного значения ARGB.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


Устанавливает цвет фона стиля.

**Remarks**

Если вы хотите задать цвет ячейки, используйте свойство Style.ForegroundColor. Это свойство будет применено только если шаблон стиля ячейки отличается от none или solid.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```


Устанавливает цвет фоновой темы.

**Remarks**

Если цвет фона не является цветом темы, будет возвращено NULL.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```


Устанавливает границы стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Граница(и), которые необходимо установить, могут быть комбинацией [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Стиль границы. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Цвет границы. |

**Returns:**
boolean - Было ли изменено текущее состояние границы.
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```


Устанавливает границы стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Граница(и), которые необходимо установить, могут быть комбинацией [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Стиль границы. |
| borderColor | [Color](../../com.aspose.cells/color) | Цвет границы. |

**Returns:**
boolean - Было ли изменено текущее состояние границы.
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```


Указывает, следует ли применять форматирование границы.

**Remarks**

Только для именованного стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckBox(boolean value) {#setCheckBox-boolean-}
```
public void setCheckBox(boolean value)
```


Указывает, является ли это стилем флажка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```


Устанавливает строку шаблона числового формата, зависящую от культуры. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроенный, будет возвращена строка шаблона, соответствующая встроенному формату.

**Remarks**

Для встроенного формата числа как содержимое шаблона (например, один встроенный формат даты — "m/d/y" для некоторых локалей, а для других локалей он становится "d/m/y"), так и спецификатор формата (например, некоторые локали используют символ, отличный от 'y', для обозначения части года в формате даты) зависят от культуры; для пользовательского пользовательского формата только спецификаторы формата изменяются в соответствии с культурой, остальные части шаблона форматирования не изменяются.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Представляет строку пользовательского числового формата этого объекта стиля. Если пользовательский числовой формат не установлен (например, формат числа встроенный), будет возвращена пустая строка "".

**Remarks**

Возвращаемая пользовательская строка не зависит от культуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```


Устанавливает пользовательскую строку числового формата ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пользовательский | java.lang.String | Строка пользовательского числового формата должна соответствовать шаблону InvariantCulture. |
| builtinPreference | boolean | Если указанная строка Custom числового формата совпадает с одним из built-in числовых форматов, соответствующих текущим региональным настройкам, следует ли установить числовой формат как built-in вместо Custom. |

### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```


Указывает, следует ли применять форматирование заливки.

**Remarks**

Только для именованного стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```


Указывает, следует ли применять форматирование шрифта.

**Remarks**

Только для именованного стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```


Устанавливает цвет переднего плана с помощью 32-битного значения ARGB.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Устанавливает цвет переднего плана стиля.

**Remarks**

Это означает отсутствие настройки цвета, если возвращено Color.Empty.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```


Устанавливает цвет темы переднего плана.

**Remarks**

Если цвет переднего плана не является цветом темы, будет возвращено NULL.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```


Представляет, будет ли формула скрыта, когда лист защищён.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```


Указывает, является ли затенение ячейки градиентным шаблоном.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Устанавливает тип горизонтального выравнивания текста в ячейке.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Представляет уровень отступа для ячейки или диапазона. Может быть только целым числом от 0 до 250.

**Remarks**

Если тип горизонтального выравнивания текста установлен в значение, отличное от left или right, уровень отступа будет сброшен до нуля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```


Указывает, следует ли использовать выравнивание ячеек по ширине или распределённое выравнивание в последней строке текста.

**Remarks**

Это типично для восточноазиатского выравнивания, но не типично в других контекстах. Работает только при распределённом горизонтальном выравнивании.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Устанавливает значение, указывающее, может ли ячейка быть изменена или нет.

**Remarks**

Блокировка ячеек не оказывает эффекта, если лист не защищён.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
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

### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```


Указывает, следует ли применять форматирование чисел.

**Remarks**

Только для именованного стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Установите контурные границы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Тип границ. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Цвет границ |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Установите контурные границы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Тип границ. |
| borderColor | [Color](../../com.aspose.cells/color) | Цвет границ |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Устанавливает тип шаблона фона ячейки.

Смотрите [BackgroundType](../../com.aspose.cells/backgroundtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```


Устанавливает цвет фона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Шаблон. |
| color1 | [Color](../../com.aspose.cells/color) | Цвет переднего плана. |
| color2 | [Color](../../com.aspose.cells/color) | Цвет фона. Работает только когда шаблон не равен BackgroundType.None и BackgroundType.Solid. |

### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```


Указывает, следует ли применять форматирование защиты.

**Remarks**

Только для именованного стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Указывает, начинается ли значение ячейки с одинарной кавычки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Представляет угол поворота текста.

**Remarks**

0: Не повернут.

255: Сверху вниз.

\-90: Вниз.

90: Вверх.

Вы можете установить 255 или значение в диапазоне от -90 до 90.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```


Представляет, автоматически ли текст уменьшается, чтобы поместиться в доступную ширину столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Представляет порядок чтения текста.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Устанавливает значение, указывающее, перенесён ли текст внутри ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```


Устанавливает указанную заливку в двухцветный градиент.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Один цвет градиента. |
| color2 | [Color](../../com.aspose.cells/color) | Два цвета градиента. |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Стиль затенения градиента. |
| вариант | int | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Устанавливает тип вертикального выравнивания текста в ячейке.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### toJson() {#toJson--}
```
public String toJson()
```


Преобразовать [Style](../../com.aspose.cells/style) в данные JSON‑структуры.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### update() {#update--}
```
public void update()
```


Примените именованный стиль к стилям ячеек, использующим этот именованный стиль. Это работает как нажатие кнопки "ok" после завершения изменения стиля. Применяется только к именованному стилю.

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

