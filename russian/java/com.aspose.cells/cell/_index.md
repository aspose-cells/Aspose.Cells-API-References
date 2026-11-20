---
title: "Ячейка"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий одну ячейку Workbook."
type: docs
url: /ru/java/com.aspose.cells/cell/
---

**Inheritance:**
java.lang.Object
```
public class Cell
```

Инкапсулирует объект, представляющий одну ячейку Workbook.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put a string into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue("Hello");
 
         String first = cell.getStringValue();
 
         //Put an integer into a cell
         cell = cells.get("B1");
         cell.putValue(12);
 
         int second = cell.getIntValue();
 
         //Put a double into a cell
         cell = cells.get(0, 2);
         cell.putValue(-1.234);
 
         double third = cell.getDoubleValue();
 
         //Put a formula into a cell
         cell = cells.get("D1");
         cell.setFormula("=B1 + C1");
 
         //Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
         cell = cells.get("b2");
         cell.setFormula("=sum(average(b1,c1), b1)");
 
         //Set style of a cell
         Style style = cell.getStyle();
         //Set background color
         style.setBackgroundColor(Color.getYellow());
         //Set format of a cell
         style.getFont().setName("Courier New");
         style.setVerticalAlignment(TextAlignmentType.TOP);
          cell.setStyle(style);
```
## Методы

| Метод | Описание |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | Вычисляет формулу ячейки. |
| [characters(int startIndex, int length)](#characters-int-int-) | Возвращает объект Characters, представляющий диапазон символов в тексте ячейки. |
| [containsExternalLink()](#containsExternalLink--) | Указывает, содержит ли эта ячейка внешнюю ссылку. |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | Копирует данные из исходной ячейки. |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | Проверяет, ссылается ли этот объект на ту же ячейку, что и другой объект ячейки. |
| [equals(Object obj)](#equals-java.lang.Object-) | Проверяет, ссылается ли этот объект на ту же ячейку, что и другой. |
| [getArrayRange()](#getArrayRange--) | Получает диапазон массива, если формула ячейки является массивной формулой. |
| [getBoolValue()](#getBoolValue--) | Получает логическое значение, содержащееся в ячейке. |
| [getCharacters()](#getCharacters--) | Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки. |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Получает номер столбца (нумерация с нуля) ячейки. |
| [getComment()](#getComment--) | Получает комментарий этой ячейки. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | Получает результат условного форматирования. |
| [getDateTimeValue()](#getDateTimeValue--) | Получает значение DateTime, содержащееся в ячейке. |
| [getDependents(boolean isAll)](#getDependents-boolean-) | Получает все ячейки, формулы которых напрямую ссылаются на эту ячейку. |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | Получает все ячейки, результат вычисления которых зависит от этой ячейки. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Получает отформатированное строковое значение этой ячейки в соответствии со стилем отображения ячейки. |
| [getDisplayStyle()](#getDisplayStyle--) | Получает стиль отображения этой ячейки. |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | Получает стиль отображения этой ячейки. |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | Получает стиль отображения этой ячейки. |
| [getDoubleValue()](#getDoubleValue--) | Получает значение double, содержащееся в ячейке. |
| [getEmbeddedImage()](#getEmbeddedImage--) | Получает встроенное изображение в ячейке. |
| [getFloatValue()](#getFloatValue--) | Получает значение float, содержащееся в ячейке. |
| [getFormatConditions()](#getFormatConditions--) | Получает условия форматирования, применяемые к этой ячейке. |
| [getFormula()](#getFormula--) | Получает формулу [Cell](../../com.aspose.cells/cell). |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | Получает формулу этой ячейки. |
| [getFormulaLocal()](#getFormulaLocal--) | Получить локализованную формулу ячейки. |
| [getHeightOfValue()](#getHeightOfValue--) | Получает высоту значения в пикселях. |
| [getHtmlString()](#getHtmlString--) | Получает HTML-строку, содержащую данные и некоторые форматы в этой ячейке. |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | Получает HTML-строку, содержащую данные и некоторые форматы в этой ячейке. |
| [getIntValue()](#getIntValue--) | Получает целочисленное значение, содержащееся в ячейке. |
| [getLeafs()](#getLeafs--) | Получить все ячейки, которые ссылаются на эту ячейку напрямую и должны быть обновлены при изменении этой ячейки. |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | Получить все ячейки, которые будут обновлены при изменении этой ячейки. |
| [getMergedRange()](#getMergedRange--) | Возвращает объект [Range](../../com.aspose.cells/range), представляющий объединённый диапазон. |
| [getName()](#getName--) | Получает имя ячейки. |
| [getNumberCategoryType()](#getNumberCategoryType--) | Представляет тип категории числового форматирования этой ячейки. |
| [getPicture()](#getPicture--) | Получает экземпляр [Picture](../../com.aspose.cells/picture), представляющий встроенное изображение в этой ячейке, или null, если в ячейке нет встроенного изображения. |
| [getPrecedents()](#getPrecedents--) | Получает все ссылки, присутствующие в формуле этой ячейки. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | Получает все предшествующие (ссылки на ячейки в текущей книге), используемые формулой этой ячейки при её вычислении. |
| [getR1C1Formula()](#getR1C1Formula--) | Получает формулу R1C1 ячейки [Cell](../../com.aspose.cells/cell). |
| [getRichValue()](#getRichValue--) | Получает расширенное значение ячейки. |
| [getRow()](#getRow--) | Получает номер строки (нумерация с нуля) ячейки. |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | Получает индекс общего стиля ячейки в пуле стилей. |
| [getStringValue()](#getStringValue--) | Получает строковое значение, содержащееся в ячейке. |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | Получает строковое значение с использованием конкретной стратегии форматирования. |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | Получает значение ячейки как строку без какого-либо форматирования. |
| [getStyle()](#getStyle--) | Получает стиль ячейки. |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | Если checkBorders равно true, проверяется, влияют ли границы других ячеек на стиль этой ячейки. |
| [getTable()](#getTable--) | Получает таблицу, содержащую эту ячейку. |
| [getType()](#getType--) | Представляет тип значения ячейки. |
| [getValidation()](#getValidation--) | Получает проверку, применённую к этой ячейке. |
| [getValidationValue()](#getValidationValue--) | Получает значение проверки, применённой к этой ячейке. |
| [getValue()](#getValue--) | Получает значение, содержащееся в этой ячейке. |
| [getWidthOfValue()](#getWidthOfValue--) | Получает ширину значения в пикселях. |
| [getWorksheet()](#getWorksheet--) | Получает родительский лист. |
| [hasCustomFunction()](#hasCustomFunction--) | Проверяет, есть ли пользовательская функция (неподдерживаемая функция) в формуле этой ячейки. |
| [hasCustomStyle()](#hasCustomStyle--) | Указывает, имеет ли эта ячейка пользовательские настройки стиля (отличные от стандартных, унаследованных от соответствующей строки, столбца или книги). |
| [hashCode()](#hashCode--) | Служит хеш-функцией для определённого типа. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Вставляет несколько символов в ячейку. |
| [isArrayFormula()](#isArrayFormula--) | Указывает, является ли формула ячейки массивной формулой. |
| [isArrayHeader()](#isArrayHeader--) | Указывает, что формула ячейки является массивной формулой и эта ячейка является первой в массиве. |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | Указывает, установлена ли эта ячейка как флажок. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | Указывает, является ли формула ячейки динамической массивной формулой (true) или устаревшей массивной формулой (false). |
| [isErrorValue()](#isErrorValue--) | Проверяет, является ли значение этой ячейки ошибкой. |
| [isFormula()](#isFormula--) | Отображает, содержит ли указанная ячейка формулу. |
| [isInArray()](#isInArray--) | Указывает, является ли формула ячейки массивной формулой. |
| [isInTable()](#isInTable--) | Указывает, является ли эта ячейка частью формулы таблицы. |
| [isMerged()](#isMerged--) | Проверяет, входит ли ячейка в объединённый диапазон. |
| [isNumericValue()](#isNumericValue--) | Указывает, является ли значение этой ячейки числовым (int, double и datetime). |
| [isRichText()](#isRichText--) | Указывает, является ли строковое значение этой ячейки текстом с расширенным форматированием. |
| [isSharedFormula()](#isSharedFormula--) | Указывает, является ли формула ячейки частью общей формулы. |
| [isStyleSet()](#isStyleSet--) | Указывает, установлен ли стиль ячейки. |
| [isTableFormula()](#isTableFormula--) | Указывает, является ли эта ячейка частью формулы таблицы. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | Помещает логическое значение в ячейку. |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | Помещает значение DateTime в ячейку. |
| [putValue(double doubleValue)](#putValue-double-) | Помещает значение double в ячейку. |
| [putValue(int intValue)](#putValue-int-) | Помещает целочисленное значение в ячейку. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Помещает объектное значение в ячейку. |
| [putValue(String stringValue)](#putValue-java.lang.String-) | Помещает строковое значение в ячейку. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Помещает строковое значение в ячейку и при необходимости преобразует его в другой тип данных. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Помещает значение в ячейку; при необходимости значение будет преобразовано к другому типу данных, а числовой формат ячейки будет сброшен. |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | Удалить формулу массива. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Заменить текст ячейки с опциями. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | Устанавливает формулу массива (устаревшую формулу массива, вводимую через CTRL+SHIFT+ENTER в MS Excel) для диапазона ячеек. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | Устанавливает формулу массива для диапазона ячеек. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Устанавливает формулу массива для диапазона ячеек. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Устанавливает формулу массива для диапазона ячеек. |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | Устанавливает форматированный текст ячейки. |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | Указывает, установлена ли эта ячейка как флажок. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | Устанавливает динамическую формулу массива и, если возможно, позволяет формуле распространяться на соседние ячейки. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | Устанавливает динамическую формулу массива и, если возможно, позволяет формуле распространяться на соседние ячейки. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | Устанавливает динамическую формулу массива и, если возможно, позволяет формуле распространяться на соседние ячейки. |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | Устанавливает встроенное изображение в ячейку. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Устанавливает формулу для [Cell](../../com.aspose.cells/cell). |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | Установить формулу и значение формулы. |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | Установить формулу и значение (рассчитанный результат) формулы. |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | Установить формулу и значение (рассчитанный результат) формулы. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Установить формулу и значение (рассчитанный результат) формулы. |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | Получить локализованную формулу ячейки. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Устанавливает HTML-строку, содержащую данные и некоторые форматы в этой ячейке. |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | Устанавливает формулу R1C1 для [Cell](../../com.aspose.cells/cell). |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | Устанавливает общие формулы для диапазона ячеек. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | Устанавливает формулу для диапазона ячеек. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Устанавливает общие формулы для диапазона ячеек. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Устанавливает общие формулы для диапазона ячеек. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Устанавливает стиль ячейки. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Применить изменённое свойство стиля к ячейке. |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Применить стиль ячейки на основе флагов. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | Создать однопараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | Создать двухпараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки. |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | Создать однопараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки. |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | Создать двухпараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Устанавливает значение, содержащееся в этой ячейке. |
| [toJson()](#toJson--) | Преобразовать [Cell](../../com.aspose.cells/cell) в данные JSON-структуры. |
| [toString()](#toString--) | Возвращает строку, представляющую текущий объект Cell. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```


Вычисляет формулу ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры расчёта |

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Возвращает объект Characters, представляющий диапазон символов в тексте ячейки.

**Remarks**

Этот метод работает только с ячейкой, содержащей строковое значение.

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Helloworld");
         cells.get("A1").characters(5, 5).getFont().setBold(true);
         cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Индекс начала символа. |
| length | int | Количество символов. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только к ячейкам с формулой.

**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```


Копирует данные из исходной ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Исходный объект [Cell](../../com.aspose.cells/cell). |

### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```


Проверяет, ссылается ли этот объект на ту же ячейку, что и другой объект ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | другой объект ячейки |

**Returns:**
логический - true, если два объекта ячейки ссылаются на одну и ту же ячейку.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Проверяет, ссылается ли этот объект на ту же ячейку, что и другой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | другой объект |

**Returns:**
логический - true, если два объекта ссылаются на одну и ту же ячейку.
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```


Получает диапазон массива, если формула ячейки является массивной формулой.

**Remarks**

Применяется только когда формула ячейки является массивной формулой.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Получает логическое значение, содержащееся в ячейке.

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки.

**Returns:**
com.aspose.cells.FontSetting[] - Все объекты Characters
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```


Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| флаг | boolean | Указывает, применять ли стиль таблицы к ячейке, если ячейка находится в таблице. |

**Returns:**
com.aspose.cells.FontSetting[] - Все объекты Characters
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
public Comment getComment()
```


Получает комментарий этой ячейки.

**Remarks**

Если к ячейке не применён комментарий, возвращает null.

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```


Получает результат условного форматирования.

**Remarks**

Возвращает null, если к этой ячейке не применено условное форматирование,

**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Получает значение DateTime, содержащееся в ячейке.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```


Получает все ячейки, формулы которых напрямую ссылаются на эту ячейку.

**Remarks**

 *  If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent.
 *  To get those formulas whose calculated results depend on this cell, please use .
 *  When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use  instead. Or, user may gather precedents map of all cells by  firstly, and then build the dependents map according to the precedents map.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         Cell[] dependents = cells.get("B1").getDependents(true);
         for (int i = 0; i <dependents.length; i++)
         {
              System.out.println(dependents[i].getName());
         }
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isAll | boolean | Указывает, проверять ли формулы в других листах. |

**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```


Получает все ячейки, результат вычисления которых зависит от этой ячейки.

**Remarks**

Чтобы использовать этот метод, убедитесь, что для рабочей книги установлено значение true для [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) и она полностью вычислена с этим параметром. Если нет ссылки на формулу в этой ячейке, будет возвращено null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("B1").getDependentsInCalculation(false);
         System.out.println("B1's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
         en = cells.get("B2").getDependentsInCalculation(false);
         System.out.println("B2's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| recursive | boolean | Возвращает ли те зависимости, которые не ссылаются напрямую на эту ячейку, а ссылаются на другие листовые элементы этой ячейки |

**Returns:**
java.util.Iterator - перечислитель для перечисления всех зависимых (объекты Cell)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Получает отформатированное строковое значение этой ячейки в соответствии со стилем отображения ячейки.

**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```


Получает стиль отображения этой ячейки.

**Remarks**

То же самое, что использование [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) для [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). То есть этот метод проверит и скорректирует верхние/нижние/левые/правые границы этой ячейки в соответствии со стилем ([getStyle()](../../com.aspose.cells/cell\#getStyle--)) её соседних ячеек, но не будет проверять объединённые ячейки и не будет проверять отображаемый стиль соседних ячеек.

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```


Получает стиль отображения этой ячейки.

**Remarks**

Если указанный флаг равен false, то поведение такое же, как у [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--). В противном случае оно соответствует использованию [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS) для [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| includeMergedBorders | boolean | Указывает, проверять ли границы объединённых ячеек. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```


Получает стиль отображения этой ячейки.

**Remarks**

Если эта ячейка также затронута другими настройками, такими как условное форматирование, объекты списка и т.д., то отображаемый стиль может отличаться от [getStyle()](../../com.aspose.cells/cell\#getStyle--).

Для флагов корректировки границ в соответствии с соседними ячейками, [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)/[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER)/[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER)/[BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) указывают, проверять и объединять нижние/верхние/правые/левые границы соседних слева/справа/сверху/снизу ячеек относительно этой.

Для повышения производительности и совместимости некоторые перечисления используются для обозначения специальных операций:

[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.

[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.

Обратите внимание, проверка границ/стилей соседних ячеек, особенно отображаемых стилей, является ресурсоёмким процессом. Если нет необходимости получать границы для возвращаемого стиля, использование [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) для отключения обработки соседних ячеек улучшит производительность. При получении границ соседних ячеек только из стилей, определённых в этих ячейках (без установки [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)), производительность также может быть лучше, поскольку проверка отображаемого стиля одной ячейки тоже затратна по времени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Указывает, какие границы необходимо проверять и корректировать в соответствии с границами соседних ячеек. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Получает значение double, содержащееся в ячейке.

**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```


Получает встроенное изображение в ячейке.

**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Получает значение float, содержащееся в ячейке.

**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```


Получает условия форматирования, применяемые к этой ячейке.

**Returns:**
com.aspose.cells.FormatConditionCollection[] - Возвращает объект [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection) object
### getFormula() {#getFormula--}
```
public String getFormula()
```


Получает формулу [Cell](../../com.aspose.cells/cell).

**Remarks**

Строка формулы всегда начинается со знака равенства (=). И, пожалуйста, всегда используйте запятую (,) в качестве разделителя параметров, например "=SUM(A1, E1, H2)".

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getFormula(boolean isR1C1, boolean isLocal) {#getFormula-boolean-boolean-}
```
public String getFormula(boolean isR1C1, boolean isLocal)
```


Получает формулу этой ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

**Returns:**
java.lang.String — формула этой ячейки.
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```


Получить локализованную формулу ячейки.

**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```


Получает высоту значения в пикселях.

**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Получает HTML-строку, содержащую данные и некоторые форматы в этой ячейке.

**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```


Получает HTML-строку, содержащую данные и некоторые форматы в этой ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| html5 | boolean | Указывает, совместимо ли значение с html5 |

**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Получает целочисленное значение, содержащееся в ячейке.

**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```


Получить все ячейки, которые ссылаются на эту ячейку напрямую и должны быть обновлены при изменении этой ячейки.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо этого, пожалуйста, используйте Cell.GetDependentsInCalculation(bool), чтобы получить всех зависимых в цепочке вычислений. Это свойство будет удалено через 12 месяцев, начиная с мая 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.util.Iterator — перечислитель для перечисления всех зависимых (Cell)
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```


Получить все ячейки, которые будут обновлены при изменении этой ячейки.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо этого, пожалуйста, используйте Cell.GetDependentsInCalculation(bool), чтобы получить всех зависимых в цепочке вычислений. Это свойство будет удалено через 12 месяцев, начиная с мая 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| recursive | boolean | Возвращает ли те листы, которые не ссылаются напрямую на эту ячейку, а ссылаются на другие листы этой ячейки |

**Returns:**
java.util.Iterator — перечислитель для перечисления всех зависимых (Cell)
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```


Возвращает объект [Range](../../com.aspose.cells/range), представляющий объединённый диапазон.

**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```


Получает имя ячейки.

**Remarks**

Имя ячейки включает букву столбца и номер строки. Например, имя ячейки в строке 0 и столбце 0 — A1.

**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```


Представляет тип категории числового форматирования этой ячейки.

Смотрите [NumberCategoryType](../../com.aspose.cells/numbercategorytype).

**Remarks**

Когда шаблон форматирования ячейки объединяется с шаблонами условного форматирования, возвращаемый тип соответствует части, используемой для текущего значения этой ячейки. Например, если шаблон форматирования для этой ячейки равен "\#,\#\#0;(\#,\#\#0);"-";@", то когда значение ячейки числовое и не равно 0, возвращаемый тип — [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\#NUMBER); когда значение ячейки равно 0 или не является числом, возвращаемый тип — [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\#TEXT).

**Returns:**
int
### getPicture() {#getPicture--}
```
public Picture getPicture()
```


Получает экземпляр [Picture](../../com.aspose.cells/picture), представляющий встроенное изображение в этой ячейке, или null, если в ячейке нет встроенного изображения.

**Returns:**
[Picture](../../com.aspose.cells/picture)
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```


Получает все ссылки, присутствующие в формуле этой ячейки.

**Remarks**

 *  Returns null if this is not a formula cell.
 *  All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.
 *  To get those references which influence the calculation only, please use .

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1");
         ReferredAreaCollection areas = cells.get("A1").getPrecedents();
         for (int i = 0; i <areas.getCount(); i++)
         {
              ReferredArea area = areas.get(i);
              StringBuilder stringBuilder = new StringBuilder();
              if (area.isExternalLink())
              {
                  stringBuilder.append("[");
                  stringBuilder.append(area.getExternalFileName());
                  stringBuilder.append("]");
              }
              stringBuilder.append(area.getSheetName());
              stringBuilder.append("!");
              stringBuilder.append(CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn()));
              if (area.isArea())
              {
                  stringBuilder.append(":");
                  stringBuilder.append(CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn()));
              }
              System.out.println(stringBuilder.toString());
         }
```

**Returns:**
[ReferredAreaCollection](../../com.aspose.cells/referredareacollection) - Collection of all references appearing in this cell's formula.
### getPrecedentsInCalculation() {#getPrecedentsInCalculation--}
```
public Iterator getPrecedentsInCalculation()
```


Получает все предшествующие (ссылки на ячейки в текущей книге), используемые формулой этой ячейки при её вычислении.

**Remarks**

Этот метод может работать только в случае, когда [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) имеет значение true для книги, и книга полностью вычислена. Если эта ячейка не является формулой или не ссылается ни на какие другие ячейки, будет возвращено null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("A2").getPrecedentsInCalculation();
         System.out.println("A2's calculation precedents:");
         while(en.hasNext())
         {
             ReferredArea r = (ReferredArea)en.next();
             System.out.println(r);
         }
```

**Returns:**
java.util.Iterator — перечислитель для перечисления всех ссылок (ReferredArea)
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```


Получает формулу R1C1 ячейки [Cell](../../com.aspose.cells/cell).

**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```


Получает расширенное значение ячейки.

**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```


Получает номер строки (нумерация с нуля) ячейки.

**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```


Получает индекс общего стиля ячейки в пуле стилей.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Получает строковое значение, содержащееся в ячейке. Если тип этой ячейки — строка, возвращается само строковое значение. Для других типов ячеек будет возвращено отформатированное строковое значение (отформатированное согласно указанному стилю этой ячейки). Отформатированное значение ячейки совпадает с тем, что вы получаете из Excel при копировании ячейки как текста (например, копирование ячейки в текстовый редактор или экспорт в csv).

**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```


Получает строковое значение с использованием конкретной стратегии форматирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy). Отформатированная стратегия. |

**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```


Получает значение ячейки как строку без какого-либо форматирования.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо этого пользователь должен получить объект значения и отформатировать его в соответствии с типом значения и конкретными требованиями. Это свойство будет удалено через 12 месяцев, начиная с декабря 2020 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Получает стиль ячейки.

**Remarks**

Чтобы изменить стиль ячейки, пожалуйста, вызовите метод Cell.SetStyle() после изменения возвращённого объекта стиля. Этот метод аналогичен [getStyle(boolean)](../../com.aspose.cells/cell\#getStyle-boolean-) с параметром true.

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```


Если checkBorders равно true, проверяется, влияют ли границы других ячеек на стиль этой ячейки.

**Remarks**

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| checkBorders | boolean | Проверьте границы других ячеек |

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```


Получает таблицу, содержащую эту ячейку.

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - 
### getType() {#getType--}
```
public int getType()
```


Представляет тип значения ячейки.

Смотрите [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```


Получает проверку, применённую к этой ячейке.

**Returns:**
[Validation](../../com.aspose.cells/validation) - 
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```


Получает значение проверки, применённой к этой ячейке.

**Returns:**
boolean -
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

Для значения типа int оно может быть возвращено как объект Integer, так и объект Double. И нет гарантии, что возвращаемое значение всегда будет сохраняться в том же типе объекта.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Получает ширину значения в пикселях.

**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Получает родительский лист.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Проверяет, есть ли пользовательская функция (неподдерживаемая функция) в формуле этой ячейки.

**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Указывает, имеет ли эта ячейка пользовательские настройки стиля (отличные от стандартных, унаследованных от соответствующей строки, столбца или книги).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Служит хеш-функцией для определённого типа.

**Returns:**
int — хеш‑код текущего объекта Cell.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Вставьте несколько символов в ячейку. Если ячейка имеет богатое форматирование, этот метод может сохранить исходное форматирование.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |
| текст | java.lang.String | Вставленный текст. |

### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Указывает, является ли формула ячейки массивной формулой.

**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```


Указывает, что формула ячейки является массивной формулой и эта ячейка является первой в массиве.

**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```


Указывает, установлена ли эта ячейка как флажок.

**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```


Указывает, является ли формула ячейки динамической массивной формулой (true) или устаревшей массивной формулой (false).

**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Проверяет, является ли значение этой ячейки ошибкой.

**Remarks**

Также применяется к ячейке с формулой для проверки, является ли вычисленный результат ошибкой.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Отображает, содержит ли указанная ячейка формулу.

**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```


Указывает, является ли формула ячейки массивной формулой.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него используйте Cell.IsArrayFormula для проверки, является ли формула ячейки массивной формулой. Это свойство будет удалено через 12 месяцев, начиная с мая 2018 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```


Указывает, является ли эта ячейка частью формулы таблицы.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него используйте Cell.IsTableFormula для проверки, является ли формула ячейки частью табличной формулы. Это свойство будет удалено через 12 месяцев, начиная с мая 2018 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```


Проверяет, входит ли ячейка в объединённый диапазон.

**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```


Указывает, является ли значение этой ячейки числовым (int, double и datetime).

**Remarks**

Также применяется к ячейке с формулой для проверки вычисленного результата

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Указывает, является ли строковое значение этой ячейки текстом с расширенным форматированием.

**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```


Указывает, является ли формула ячейки частью общей формулы.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Указывает, установлен ли стиль ячейки. Если возвращается false, это означает, что у ячейки используется формат по умолчанию.

**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```


Указывает, является ли эта ячейка частью формулы таблицы.

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




### putValue(boolean boolValue) {#putValue-boolean-}
```
public void putValue(boolean boolValue)
```


Помещает логическое значение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```


Помещает значение DateTime в ячейку.

**Remarks**

Установка значения DateTime для ячейки не означает, что ячейка автоматически будет отформатирована как дата и время. Значение DateTime хранится как числовое значение в модели данных как MS Excel, так и Aspose.Cells. Будет ли числовое значение интерпретировано как само число или как дата и время, зависит от применённого к ячейке числового формата. Если ячейка не отформатирована как дата и время, она будет отображаться как числовое значение, даже если вы ввели DateTime.

**Example**

Этот пример показывает, как установить значение DateTime в ячейку и заставить его отображаться как дата и время.

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put date time into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue(new DateTime(2023, 5, 15));
         Style style = cell.getStyle(false);
         style.setNumber(14);
         cell.setStyle(style);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Входное значение |

### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```


Помещает значение double в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| doubleValue | double | Входное значение |

### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```


Помещает целочисленное значение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| intValue | int | Входное значение |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Помещает объектное значение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| objectValue | java.lang.Object | входное значение |

### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```


Помещает строковое значение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | java.lang.String | Входное значение |

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

### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```


Удалить формулу массива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| leaveNormalFormula | boolean | True обозначает преобразование массивной формулы в обычную формулу. |

### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```


Заменить текст ячейки с опциями.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | java.lang.String | Заполнитель ячейки |
| newValue | java.lang.String | Строковое значение для замены |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Параметры замены |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```


Устанавливает формулу массива (устаревшую формулу массива, вводимую через CTRL+SHIFT+ENTER в MS Excel) для диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | java.lang.String | Массивная формула. |
| rowNumber | int | Количество строк для заполнения результата массивной формулы. |
| columnNumber | int | Количество столбцов для заполнения результата массивной формулы. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Устанавливает формулу массива для диапазона ячеек.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Это свойство будет удалено через 12 месяцев, начиная с декабря 2019 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | java.lang.String | Массивная формула. |
| rowNumber | int | Количество строк для заполнения результата массивной формулы. |
| columnNumber | int | Количество столбцов для заполнения результата массивной формулы. |
| isR1C1 | boolean | является ли формула формулой R1C1 |
| isLocal | boolean | является ли формула отформатирована в соответствии с локалью |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Устанавливает формулу массива для диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | java.lang.String | Массивная формула. |
| rowNumber | int | Количество строк для заполнения результата массивной формулы. |
| columnNumber | int | Количество столбцов для заполнения результата массивной формулы. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Параметры разбора формулы. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Устанавливает формулу массива для диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | java.lang.String | Массивная формула. |
| rowNumber | int | Количество строк для заполнения результата массивной формулы. |
| columnNumber | int | Количество столбцов для заполнения результата массивной формулы. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Параметры разбора формулы. |
| значения | java.lang.Object[][] | значения для ячеек с заданной массивной формулой |

### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```


Устанавливает форматированный текст ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | Все объекты Characters. |

### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```


Указывает, установлена ли эта ячейка как флажок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```


Устанавливает динамическую формулу массива и, если возможно, позволяет формуле распространяться на соседние ячейки.

**Remarks**

возвращаемый диапазон может не совпадать с фактическим диапазоном, в который эта динамическая массивная формула распространяется. Если в диапазоне есть непустые ячейки, формула будет установлена только для текущей ячейки и помечена как "\#SPILL!". Однако в такой ситуации мы всё равно возвращаем весь диапазон, в который должна распространяться формула.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | java.lang.String | выражение формулы |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | параметры разбора формулы. Параметр "Parse" будет игнорироваться, и формула всегда будет разбираться немедленно |
| calculateValue | boolean | нужно ли вычислять эту динамическую массивную формулу для ячеек в распространённом диапазоне. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```


Устанавливает динамическую формулу массива и, если возможно, позволяет формуле распространяться на соседние ячейки.

**Remarks**

возвращаемый диапазон может не совпадать с фактическим диапазоном, в который эта динамическая массивная формула распространяется. Если в диапазоне есть непустые ячейки, формула будет установлена только для текущей ячейки и помечена как "\#SPILL!". Однако в такой ситуации мы всё равно возвращаем весь диапазон, в который должна распространяться формула.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | java.lang.String | выражение формулы |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | параметры разбора формулы. Параметр "Parse" будет игнорироваться, и формула всегда будет разбираться немедленно |
| значения | java.lang.Object[][] | значения (вычисленные результаты) для ячеек с заданной динамической массивной формулой |
| calculateRange | boolean | Нужно ли вычислять распространённый диапазон для этой динамической массивной формулы. Если параметр "values" не равен null и этот флаг установлен в false, то высота распространённого диапазона будет values.Length, а ширина — values[0].Length. |
| calculateValue | boolean | нужно ли вычислять эту динамическую массивную формулу для ячеек в распространённом диапазоне, когда "values" равно null или соответствующий элемент в "values" для одной ячейки равен null. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```


Устанавливает динамическую формулу массива и, если возможно, позволяет формуле распространяться на соседние ячейки.

**Remarks**

возвращаемый диапазон может не совпадать с фактическим диапазоном, в который эта динамическая массивная формула распространяется. Если в диапазоне есть непустые ячейки, формула будет установлена только для текущей ячейки и помечена как "\#SPILL!". Однако в такой ситуации мы всё равно возвращаем весь диапазон, в который должна распространяться формула.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | java.lang.String | выражение формулы |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | параметры разбора формулы. Параметр "Parse" будет игнорироваться, и формула всегда будет разбираться немедленно |
| значения | java.lang.Object[][] | значения (вычисленные результаты) для ячеек с заданной динамической массивной формулой |
| calculateRange | boolean | Нужно ли вычислять распространённый диапазон для этой динамической массивной формулы. Если параметр "values" не равен null и этот флаг установлен в false, то высота распространённого диапазона будет values.Length, а ширина — values[0].Length. |
| calculateValue | boolean | нужно ли вычислять эту динамическую массивную формулу для ячеек в распространённом диапазоне, когда "values" равно null или соответствующий элемент в "values" для одной ячейки равен null. |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры вычисления формулы. Обычно, с учётом производительности, свойство [CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\#getRecursive--) должно быть false. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```


Устанавливает встроенное изображение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Устанавливает формулу для [Cell](../../com.aspose.cells/cell).

**Remarks**

Строка формулы всегда начинается со знака равенства (=). И, пожалуйста, всегда используйте запятую (,) в качестве разделителя параметров, например "=SUM(A1, E1, H2)".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```


Установить формулу и значение формулы.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте Cell.SetFormula(string,FormulaParseOptions,object). Это свойство будет удалено через 12 месяцев, начиная с декабря 2019 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула. |
| isR1C1 | boolean | Является ли формула формулой R1C1. |
| isLocal | boolean | Отформатирована ли формула в соответствии с локалью. |
| значение | java.lang.Object | Значение формулы. |

### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```


Установить формулу и значение (рассчитанный результат) формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Параметры разбора формулы. |

### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```


Установить формулу и значение (рассчитанный результат) формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Параметры разбора формулы. |
| значение | java.lang.Object | Значение (вычисленный результат) формулы. |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Установить формулу и значение (рассчитанный результат) формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула. |
| значение | java.lang.Object | Значение (вычисленный результат) формулы. |

### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```


Получить локализованную формулу ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Устанавливает HTML-строку, содержащую данные и некоторые форматы в этой ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```


Устанавливает формулу R1C1 для [Cell](../../com.aspose.cells/cell).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```


Устанавливает общие формулы для диапазона ячеек.

**Remarks**

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sharedFormula | java.lang.String | Общая формула. |
| rowNumber | int | Количество строк для заполнения формулы. |
| columnNumber | int | Количество столбцов для заполнения формулы. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Устанавливает формулу для диапазона ячеек.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо этого, пожалуйста, используйте Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Это свойство будет удалено через 12 месяцев, начиная с декабря 2019 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sharedFormula | java.lang.String | Общая формула. |
| rowNumber | int | Количество строк для заполнения формулы. |
| columnNumber | int | Количество столбцов для заполнения формулы. |
| isR1C1 | boolean | является ли формула формулой R1C1 |
| isLocal | boolean | является ли формула отформатирована в соответствии с локалью |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Устанавливает общие формулы для диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sharedFormula | java.lang.String | Общая формула. |
| rowNumber | int | Количество строк для заполнения формулы. |
| columnNumber | int | Количество столбцов для заполнения формулы. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Параметры разбора формулы. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Устанавливает общие формулы для диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sharedFormula | java.lang.String | Общая формула. |
| rowNumber | int | Количество строк для заполнения формулы. |
| columnNumber | int | Количество столбцов для заполнения формулы. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Параметры разбора формулы. |
| значения | java.lang.Object[][] | значения для этих ячеек с заданной общей формулой |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Устанавливает стиль ячейки.

**Remarks**

Если настройки границы изменены, граница корректируемых ячеек также будет обновлена.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Стиль ячейки. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Применить изменённое свойство стиля к ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Стиль ячейки. |
| explicitFlag | boolean | True, только перезаписывая форматирование, которое явно задано. |

### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```


Применить стиль ячейки на основе флагов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Стиль ячейки. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаг стиля. |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```


Создать однопараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowNumber | int | Количество строк для заполнения формулы. |
| columnNumber | int | Количество столбцов для заполнения формулы. |
| rowIndexOfInputCell | int | индекс строки входной ячейки |
| columnIndexOfInputCell | int | индекс столбца входной ячейки |
| isRowInput | boolean | Указывает, является ли входная ячейка ячейкой ввода строки (true) или ячейкой ввода столбца (false). |
| значения | java.lang.Object[][] | значения для ячеек в диапазоне формулы таблицы |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```


Создать двухпараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowNumber | int | Количество строк для заполнения формулы. |
| columnNumber | int | Количество столбцов для заполнения формулы. |
| rowIndexOfRowInputCell | int | индекс строки ячейки ввода строки |
| columnIndexOfRowInputCell | int | индекс столбца ячейки ввода строки |
| rowIndexOfColumnInputCell | int | индекс строки ячейки ввода столбца |
| columnIndexOfColumnInputCell | int | индекс столбца ячейки ввода столбца |
| значения | java.lang.Object[][] | значения для ячеек в диапазоне формулы таблицы |

### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```


Создать однопараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowNumber | int | Количество строк для заполнения формулы. |
| columnNumber | int | Количество столбцов для заполнения формулы. |
| inputCell | java.lang.String | входная ячейка |
| isRowInput | boolean | Указывает, является ли входная ячейка ячейкой ввода строки (true) или ячейкой ввода столбца (false). |
| значения | java.lang.Object[][] | значения для ячеек в диапазоне формулы таблицы |

### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```


Создать двухпараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowNumber | int | Количество строк для заполнения формулы. |
| columnNumber | int | Количество столбцов для заполнения формулы. |
| rowInputCell | java.lang.String | ячейка ввода строки |
| columnInputCell | java.lang.String | ячейка ввода столбца |
| значения | java.lang.Object[][] | значения для ячеек в диапазоне формулы таблицы |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Устанавливает значение, содержащееся в этой ячейке.

**Remarks**

Возможный тип:

null,

Boolean,

DateTime,

Double,

Integer

String.

Для значения типа int оно может быть возвращено как объект Integer, так и объект Double. И нет гарантии, что возвращаемое значение всегда будет сохраняться в том же типе объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### toJson() {#toJson--}
```
public String toJson()
```


Преобразовать [Cell](../../com.aspose.cells/cell) в данные JSON-структуры.

**Returns:**
java.lang.String -
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

