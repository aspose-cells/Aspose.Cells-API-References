---
title: "单元格"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示单个工作簿单元格的对象。"
type: docs
url: /zh/java/com.aspose.cells/cell/
---

**Inheritance:**
java.lang.Object
```
public class Cell
```

封装表示单个工作簿单元格的对象。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | 计算单元格的公式。 |
| [characters(int startIndex, int length)](#characters-int-int-) | 返回一个 Characters 对象，表示单元格文本中字符范围。 |
| [containsExternalLink()](#containsExternalLink--) | 指示此单元格是否包含外部链接。 |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | 从源单元格复制数据。 |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | 检查此对象是否与另一个单元格对象引用相同的单元格。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 检查此对象是否与另一个引用相同的单元格。 |
| [getArrayRange()](#getArrayRange--) | 如果单元格的公式是数组公式，则获取数组范围。 |
| [getBoolValue()](#getBoolValue--) | 获取单元格中包含的布尔值。 |
| [getCharacters()](#getCharacters--) | 返回所有表示单元格文本中字符范围的 Characters 对象。 |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | 返回所有表示单元格文本中字符范围的 Characters 对象。 |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | 获取单元格的列号（从零开始）。 |
| [getComment()](#getComment--) | 获取此单元格的注释。 |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | 获取条件格式的结果。 |
| [getDateTimeValue()](#getDateTimeValue--) | 获取单元格中包含的 DateTime 值。 |
| [getDependents(boolean isAll)](#getDependents-boolean-) | 获取所有公式直接引用此单元格的单元格。 |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | 获取所有计算结果依赖于此单元格的单元格。 |
| [getDisplayStringValue()](#getDisplayStringValue--) | 获取此单元格按显示样式格式化后的字符串值。 |
| [getDisplayStyle()](#getDisplayStyle--) | 获取此单元格的显示样式。 |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | 获取此单元格的显示样式。 |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | 获取此单元格的显示样式。 |
| [getDoubleValue()](#getDoubleValue--) | 获取单元格中包含的 double 值。 |
| [getEmbeddedImage()](#getEmbeddedImage--) | 获取单元格中嵌入的图像。 |
| [getFloatValue()](#getFloatValue--) | 获取单元格中包含的 float 值。 |
| [getFormatConditions()](#getFormatConditions--) | 获取适用于此单元格的格式条件。 |
| [getFormula()](#getFormula--) | 获取 [Cell](../../com.aspose.cells/cell) 的公式。 |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | 获取此单元格的公式。 |
| [getFormulaLocal()](#getFormulaLocal--) | 获取单元格的本地化格式公式。 |
| [getHeightOfValue()](#getHeightOfValue--) | 获取该值的高度，单位为像素。 |
| [getHtmlString()](#getHtmlString--) | 获取包含此单元格数据和部分格式的 html 字符串。 |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | 获取包含此单元格数据和部分格式的 html 字符串。 |
| [getIntValue()](#getIntValue--) | 获取单元格中包含的整数值。 |
| [getLeafs()](#getLeafs--) | 获取所有直接引用此单元格且在此单元格修改时需要更新的单元格。 |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | 获取在此单元格修改时将被更新的所有单元格。 |
| [getMergedRange()](#getMergedRange--) | 返回表示合并范围的 [Range](../../com.aspose.cells/range) 对象。 |
| [getName()](#getName--) | 获取单元格的名称。 |
| [getNumberCategoryType()](#getNumberCategoryType--) | 表示此单元格数字格式的类别类型。 |
| [getPicture()](#getPicture--) | 获取一个 [Picture](../../com.aspose.cells/picture) 实例，用于表示此单元格中的嵌入图像；如果该单元格没有嵌入图像，则返回 null。 |
| [getPrecedents()](#getPrecedents--) | 获取此单元格公式中出现的所有引用。 |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | 获取此单元格公式在计算时使用的所有前置单元格（对当前工作簿中单元格的引用）。 |
| [getR1C1Formula()](#getR1C1Formula--) | 获取 [Cell](../../com.aspose.cells/cell) 的 R1C1 公式。 |
| [getRichValue()](#getRichValue--) | 获取单元格的富值。 |
| [getRow()](#getRow--) | 获取单元格的行号（从零开始）。 |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | 获取单元格在样式池中的共享样式索引。 |
| [getStringValue()](#getStringValue--) | 获取单元格中包含的字符串值。 |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | 按特定格式化策略获取字符串值。 |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | 获取单元格的值为字符串，且不使用任何格式。 |
| [getStyle()](#getStyle--) | 获取单元格样式。 |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | 如果 checkBorders 为 true，则检查其他单元格的边框是否会影响此单元格的样式。 |
| [getTable()](#getTable--) | 获取包含此单元格的表格。 |
| [getType()](#getType--) | 表示单元格值的类型。 |
| [getValidation()](#getValidation--) | 获取应用于此单元格的验证。 |
| [getValidationValue()](#getValidationValue--) | 获取应用于此单元格的验证的值。 |
| [getValue()](#getValue--) | 获取此单元格中包含的值。 |
| [getWidthOfValue()](#getWidthOfValue--) | 获取该值的宽度，单位为像素。 |
| [getWorksheet()](#getWorksheet--) | 获取父工作表。 |
| [hasCustomFunction()](#hasCustomFunction--) | 检查此单元格公式中是否存在自定义函数（不受支持的函数）。 |
| [hasCustomStyle()](#hasCustomStyle--) | 指示此单元格是否具有自定义样式设置（不同于从相应行、列或工作簿继承的默认设置）。 |
| [hashCode()](#hashCode--) | 作为特定类型的哈希函数。 |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | 向单元格插入一些字符。 |
| [isArrayFormula()](#isArrayFormula--) | 指示单元格公式是否为数组公式。 |
| [isArrayHeader()](#isArrayHeader--) | 指示单元格的公式是数组公式且是该数组的首个单元格。 |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | 指示是否将此单元格设置为复选框。 |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | 指示单元格的公式是动态数组公式（true）还是传统数组公式（false）。 |
| [isErrorValue()](#isErrorValue--) | 检查此单元格的值是否为错误。 |
| [isFormula()](#isFormula--) | 表示指定的单元格是否包含公式。 |
| [isInArray()](#isInArray--) | 指示单元格公式是否为数组公式。 |
| [isInTable()](#isInTable--) | 指示此单元格是否是表格公式的一部分。 |
| [isMerged()](#isMerged--) | 检查单元格是否是合并范围的一部分。 |
| [isNumericValue()](#isNumericValue--) | 指示此单元格的值是否为数值（int、double 和 datetime） |
| [isRichText()](#isRichText--) | 指示此单元格的字符串值是否为富格式文本。 |
| [isSharedFormula()](#isSharedFormula--) | 指示单元格公式是否是共享公式的一部分。 |
| [isStyleSet()](#isStyleSet--) | 指示是否已设置单元格的样式。 |
| [isTableFormula()](#isTableFormula--) | 指示此单元格是否是表格公式的一部分。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | 将布尔值写入单元格。 |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | 将 DateTime 值写入单元格。 |
| [putValue(double doubleValue)](#putValue-double-) | 将 double 值写入单元格。 |
| [putValue(int intValue)](#putValue-int-) | 将整数值写入单元格。 |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | 将对象值写入单元格。 |
| [putValue(String stringValue)](#putValue-java.lang.String-) | 将字符串值写入单元格。 |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | 将字符串值写入单元格，并在适当时将其转换为其他数据类型。 |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | 将值写入单元格，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。 |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | 删除数组公式。 |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | 使用选项替换单元格的文本。 |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | 为一组单元格设置数组公式（通过在 MS Excel 中按 CTRL+SHIFT+ENTER 输入的传统数组公式）。 |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | 为一组单元格设置数组公式。 |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | 为一组单元格设置数组公式。 |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | 为一组单元格设置数组公式。 |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | 设置单元格的富文本格式。 |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | 指示是否将此单元格设置为复选框。 |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | 设置动态数组公式，并在可能的情况下使公式溢出到相邻单元格。 |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | 设置动态数组公式，并在可能的情况下使公式溢出到相邻单元格。 |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | 设置动态数组公式，并在可能的情况下使公式溢出到相邻单元格。 |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | 设置单元格中的嵌入图像。 |
| [setFormula(String value)](#setFormula-java.lang.String-) | 设置 [Cell](../../com.aspose.cells/cell) 的公式。 |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | 设置公式及公式的值。 |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | 设置公式及公式的值（计算结果）。 |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | 设置公式及公式的值（计算结果）。 |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | 设置公式及公式的值（计算结果）。 |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | 获取单元格的本地化格式公式。 |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | 设置包含数据和某些格式的 HTML 字符串到此单元格。 |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | 设置 [Cell](../../com.aspose.cells/cell) 的 R1C1 公式。 |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | 为一系列单元格设置共享公式。 |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | 为一系列单元格设置公式。 |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | 为一系列单元格设置共享公式。 |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | 为一系列单元格设置共享公式。 |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | 设置单元格样式。 |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | 将样式的已更改属性应用到单元格。 |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | 根据标志应用单元格样式。 |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | 从此单元格开始，为给定范围创建单变量数据表。 |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | 从此单元格开始，为给定范围创建双变量数据表。 |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | 从此单元格开始，为给定范围创建单变量数据表。 |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | 从此单元格开始，为给定范围创建双变量数据表。 |
| [setValue(Object value)](#setValue-java.lang.Object-) | 设置此单元格中包含的值。 |
| [toJson()](#toJson--) | 将 [Cell](../../com.aspose.cells/cell) 转换为 JSON 结构数据。 |
| [toString()](#toString--) | 返回表示当前 Cell 对象的字符串。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```


计算单元格的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 计算的选项 |

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


返回一个 Characters 对象，表示单元格文本中字符范围。

**Remarks**

此方法仅适用于具有字符串值的单元格。

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Helloworld");
         cells.get("A1").characters(5, 5).getFont().setBold(true);
         cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 字符起始位置的索引。 |
| length | int | 字符数。 |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


指示此单元格是否包含外部链接。仅在单元格为公式单元格时适用。

**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```


从源单元格复制数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | 源 [Cell](../../com.aspose.cells/cell) 对象。 |

### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```


检查此对象是否与另一个单元格对象引用相同的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | 另一个单元格对象 |

**Returns:**
布尔值 - 如果两个单元格对象引用同一单元格则为 true。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


检查此对象是否与另一个引用相同的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 另一个对象 |

**Returns:**
布尔值 - 如果两个对象引用同一单元格则为 true。
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```


如果单元格的公式是数组公式，则获取数组范围。

**Remarks**

仅在单元格的公式为数组公式时适用

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


获取单元格中包含的布尔值。

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


返回所有表示单元格文本中字符范围的 Characters 对象。

**Returns:**
com.aspose.cells.FontSetting[] - 所有字符对象
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```


返回所有表示单元格文本中字符范围的 Characters 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标志 | boolean | 指示如果单元格位于表中，是否对其应用表样式。 |

**Returns:**
com.aspose.cells.FontSetting[] - 所有字符对象
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


获取单元格的列号（从零开始）。

**Returns:**
int
### getComment() {#getComment--}
```
public Comment getComment()
```


获取此单元格的注释。

**Remarks**

如果没有适用于单元格的批注，则返回 null。

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```


获取条件格式的结果。

**Remarks**

如果未对该单元格应用条件格式，则返回 null，

**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


获取单元格中包含的 DateTime 值。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```


获取所有公式直接引用此单元格的单元格。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isAll | boolean | 指示是否检查其他工作表中的公式 |

**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```


获取所有计算结果依赖于此单元格的单元格。

**Remarks**

要使用此方法，请确保工作簿已将 [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) 设置为 true，并已使用此设置完成全部计算。如果没有公式引用此单元格，将返回 null。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| recursive | boolean | 是否返回那些不直接引用此单元格但引用此单元格其他叶子单元格的从属项 |

**Returns:**
java.util.Iterator - 用于枚举所有从属项（单元格对象）的枚举器
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


获取此单元格按显示样式格式化后的字符串值。

**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```


获取此单元格的显示样式。

**Remarks**

与在 [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-) 中使用 [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) 的效果相同。即，此方法将根据相邻单元格的样式（[getStyle()](../../com.aspose.cells/cell\#getStyle--)）检查并调整该单元格的上/下/左/右边框，但不检查合并单元格，也不检查相邻单元格的显示样式。

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```


获取此单元格的显示样式。

**Remarks**

如果指定的标志为 false，则等同于 [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--) 的行为。否则等同于在 [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-) 中使用 [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| includeMergedBorders | boolean | 指示是否检查合并单元格的边框。 |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```


获取此单元格的显示样式。

**Remarks**

如果此单元格还受到条件格式、列表对象等其他设置的影响，则显示样式可能与 [getStyle()](../../com.aspose.cells/cell\#getStyle--) 不同。

用于根据相邻单元格调整边框的标志，[BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)、[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER)、[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER) 和 [BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) 表示是否检查并合并左/右/上/下相邻单元格的底部/顶部/右侧/左侧边框。

出于性能和兼容性考虑，使用了一些枚举来表示特定操作：

[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.

[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.

请注意，检查相邻单元格的边框/样式，尤其是显示样式，是一个耗时的过程。如果不需要获取返回样式的边框，使用 [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) 来禁用相邻单元格的处理可提升性能。当仅从这些单元格上定义的样式（未设置 [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)）获取相邻单元格的边框时，性能也可能更好，因为检查单个单元格的显示样式同样耗时。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype)。指示需要根据相邻单元格的边框进行检查和调整的边框。 |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


获取单元格中包含的 double 值。

**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```


获取单元格中嵌入的图像。

**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


获取单元格中包含的 float 值。

**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```


获取适用于此单元格的格式条件。

**Returns:**
com.aspose.cells.FormatConditionCollection[] - 返回 [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection) 对象
### getFormula() {#getFormula--}
```
public String getFormula()
```


获取 [Cell](../../com.aspose.cells/cell) 的公式。

**Remarks**

公式字符串总是以等号 (=) 开头。并请始终使用逗号 (,) 作为参数分隔符，例如 "=SUM(A1, E1, H2)"。

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


获取此单元格的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

**Returns:**
java.lang.String - 此单元格的公式。
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```


获取单元格的本地化格式公式。

**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```


获取该值的高度，单位为像素。

**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


获取包含此单元格数据和部分格式的 html 字符串。

**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```


获取包含此单元格数据和部分格式的 html 字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| html5 | boolean | 指示该值是否兼容 html5 |

**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


获取单元格中包含的整数值。

**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```


获取所有直接引用此单元格且在此单元格修改时需要更新的单元格。

**Remarks**

注意：此类已过时。请改用 Cell.GetDependentsInCalculation(bool) 来获取计算链中的所有从属项。此属性将在自 2022 年 5 月起的 12 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
java.util.Iterator - 用于枚举所有从属项（单元格）的枚举器
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```


获取在此单元格修改时将被更新的所有单元格。

**Remarks**

注意：此类已过时。请改用 Cell.GetDependentsInCalculation(bool) 来获取计算链中的所有从属项。此属性将在自 2022 年 5 月起的 12 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| recursive | boolean | 是否返回那些不直接引用此单元格但引用此单元格其他叶子单元格的叶子项 |

**Returns:**
java.util.Iterator - 用于枚举所有从属项（单元格）的枚举器
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```


返回表示合并范围的 [Range](../../com.aspose.cells/range) 对象。

**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```


获取单元格的名称。

**Remarks**

单元格名称由其列字母和行号组成。例如，位于第 0 行第 0 列的单元格名称是 A1。

**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```


表示此单元格数字格式的类别类型。

参见 [NumberCategoryType](../../com.aspose.cells/numbercategorytype)。

**Remarks**

当单元格的格式化模式与条件格式化模式结合时，返回的类型对应于用于该单元格当前值的那部分。例如，如果该单元格的格式化模式是 "\\#,\\#\\#0;(\\#,\\#\\#0);"-";@"，则当单元格的值为数值且不为 0 时，返回的类型是 [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\\#NUMBER)；当单元格的值为 0 或非数值时，返回的类型是 [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\\#TEXT)。

**Returns:**
int
### getPicture() {#getPicture--}
```
public Picture getPicture()
```


获取一个 [Picture](../../com.aspose.cells/picture) 实例，用于表示此单元格中的嵌入图像；如果该单元格没有嵌入图像，则返回 null。

**Returns:**
[Picture](../../com.aspose.cells/picture)
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```


获取此单元格公式中出现的所有引用。

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


获取此单元格公式在计算时使用的所有前置单元格（对当前工作簿中单元格的引用）。

**Remarks**

此方法只能在工作簿的 [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\\#getEnableCalculationChain--) 为 true 且工作簿已完成全部计算的情况下使用。如果该单元格不是公式或不引用任何其他单元格，将返回 null。

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
java.util.Iterator - 用于枚举所有引用（ReferredArea）的枚举器
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```


获取 [Cell](../../com.aspose.cells/cell) 的 R1C1 公式。

**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```


获取单元格的富值。

**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```


获取单元格的行号（从零开始）。

**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```


获取单元格在样式池中的共享样式索引。

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


获取单元格中包含的字符串值。如果该单元格的类型是字符串，则返回字符串本身。对于其他单元格类型，将返回格式化后的字符串值（使用此单元格指定的样式进行格式化）。格式化后的单元格值与在 Excel 中复制单元格为文本时（例如复制到文本编辑器或导出为 csv）得到的值相同。

**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```


按特定格式化策略获取字符串值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy)。已格式化的策略。 |

**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```


获取单元格的值为字符串，且不使用任何格式。

**Remarks**

注意：此方法现已过时。请改为获取值对象并根据值类型和具体需求进行格式化。此属性将在自 2020 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```


获取单元格样式。

**Remarks**

要更改单元格的样式，请在修改返回的样式对象后调用 `Cell.SetStyle()` 方法。此方法等同于使用参数为 true 的 [getStyle(boolean)](../../com.aspose.cells/cell\\#getStyle-boolean-)。

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```


如果 checkBorders 为 true，则检查其他单元格的边框是否会影响此单元格的样式。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| checkBorders | boolean | 检查其他单元格的边框 |

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```


获取包含此单元格的表格。

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - 
### getType() {#getType--}
```
public int getType()
```


表示单元格值的类型。

参见 [CellValueType](../../com.aspose.cells/cellvaluetype)。

**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```


获取应用于此单元格的验证。

**Returns:**
[Validation](../../com.aspose.cells/validation) - 
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```


获取应用于此单元格的验证的值。

**Returns:**
boolean -
### getValue() {#getValue--}
```
public Object getValue()
```


获取此单元格中包含的值。

**Remarks**

可能的类型：

null，

Boolean，

DateTime，

Double，

Integer

String。

对于 int 值，可能返回 Integer 对象或 Double 对象。且无法保证返回的值始终保持相同的对象类型。

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


获取该值的宽度，单位为像素。

**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


获取父工作表。

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


检查此单元格公式中是否存在自定义函数（不受支持的函数）。

**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


指示此单元格是否具有自定义样式设置（不同于从相应行、列或工作簿继承的默认设置）。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


作为特定类型的哈希函数。

**Returns:**
int - 当前 Cell 对象的哈希码。
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


向单元格插入一些字符。如果单元格是富格式的，此方法可以保留原始格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |
| 文本 | java.lang.String | 已插入的文本。 |

### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


指示单元格公式是否为数组公式。

**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```


指示单元格的公式是数组公式且是该数组的首个单元格。

**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```


指示是否将此单元格设置为复选框。

**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```


指示单元格的公式是动态数组公式（true）还是传统数组公式（false）。

**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


检查此单元格的值是否为错误。

**Remarks**

同样适用于公式单元格，以检查计算结果是否为错误。

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


表示指定的单元格是否包含公式。

**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```


指示单元格公式是否为数组公式。

**Remarks**

注意：此类现已过时。请改用 Cell.IsArrayFormula 来检查单元格公式是否为数组公式。此属性将在自 2018 年 5 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```


指示此单元格是否是表格公式的一部分。

**Remarks**

注意：此类现已过时。请改用 Cell.IsTableFormula 来检查单元格公式是否为表格公式的一部分。此属性将在自 2018 年 5 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```


检查单元格是否是合并范围的一部分。

**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```


指示此单元格的值是否为数值（int、double 和 datetime）

**Remarks**

同样适用于公式单元格，以检查计算结果

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


指示此单元格的字符串值是否为富格式文本。

**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```


指示单元格公式是否是共享公式的一部分。

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


指示单元格的样式是否已设置。如果返回 false，则表示该单元格使用默认的单元格格式。

**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```


指示此单元格是否是表格公式的一部分。

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


将布尔值写入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```


将 DateTime 值写入单元格。

**Remarks**

为单元格设置 DateTime 值并不意味着单元格会自动格式化为日期时间。DateTime 值在 MS Excel 和 Aspose.Cells 的数据模型中都以数值形式存储。数值是否被视为数值本身或日期时间取决于该单元格应用的数字格式。如果该单元格未被格式化为日期时间，即使您输入的是 DateTime，也会显示为数值。

**Example**

此示例展示了如何将 DateTime 值设置到单元格并使其显示为日期时间。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | 输入值 |

### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```


将 double 值写入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| doubleValue | double | 输入值 |

### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```


将整数值写入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| intValue | int | 输入值 |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


将对象值写入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| objectValue | java.lang.Object | 输入值 |

### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```


将字符串值写入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringValue | java.lang.String | 输入值 |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


将字符串值写入单元格，并在适当时将其转换为其他数据类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringValue | java.lang.String | 输入值 |
| isConverted | boolean | True: 如适用，转换为其他数据类型。 |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


将值写入单元格，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringValue | java.lang.String | 输入值 |
| isConverted | boolean | True: 如适用，转换为其他数据类型。 |
| setStyle | boolean | True: 在转换为其他数据类型时将数字格式设置为单元格的样式 |

### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```


删除数组公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| leaveNormalFormula | boolean | True 表示将数组公式转换为普通公式。 |

### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```


使用选项替换单元格的文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | java.lang.String | 单元格占位符 |
| newValue | java.lang.String | 要替换的字符串值 |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | 替换选项 |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```


为一组单元格设置数组公式（通过在 MS Excel 中按 CTRL+SHIFT+ENTER 输入的传统数组公式）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arrayFormula | java.lang.String | 数组公式。 |
| rowNumber | int | 用于填充数组公式结果的行数。 |
| columnNumber | int | 用于填充数组公式结果的列数。 |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


为一组单元格设置数组公式。

**Remarks**

注意：此类已过时。请改用 Cell.SetArrayFormula(string,int,int,FormulaParseOptions)。此属性将在自 2019 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arrayFormula | java.lang.String | 数组公式。 |
| rowNumber | int | 用于填充数组公式结果的行数。 |
| columnNumber | int | 用于填充数组公式结果的列数。 |
| isR1C1 | boolean | 公式是否为 R1C1 公式 |
| isLocal | boolean | 公式是否为本地化格式 |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


为一组单元格设置数组公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arrayFormula | java.lang.String | 数组公式。 |
| rowNumber | int | 用于填充数组公式结果的行数。 |
| columnNumber | int | 用于填充数组公式结果的列数。 |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。 |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


为一组单元格设置数组公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arrayFormula | java.lang.String | 数组公式。 |
| rowNumber | int | 用于填充数组公式结果的行数。 |
| columnNumber | int | 用于填充数组公式结果的列数。 |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。 |
| 值 | java.lang.Object[][] | 具有给定数组公式的单元格的值 |

### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```


设置单元格的富文本格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | 所有 Characters 对象。 |

### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```


指示是否将此单元格设置为复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```


设置动态数组公式，并在可能的情况下使公式溢出到相邻单元格。

**Remarks**

返回的范围可能与此动态数组公式实际溢出的范围不同。如果范围内有非空单元格，公式将仅设置在当前单元格并标记为 "\\#SPILL!"。但对于此类情况，我们仍返回该公式应溢出的整个范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arrayFormula | java.lang.String | 公式表达式 |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。\"Parse\" 选项将被忽略，公式将始终立即解析 |
| calculateValue | boolean | 是否为溢出范围内的单元格计算此动态数组公式。 |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```


设置动态数组公式，并在可能的情况下使公式溢出到相邻单元格。

**Remarks**

返回的范围可能与此动态数组公式实际溢出的范围不同。如果范围内有非空单元格，公式将仅设置在当前单元格并标记为 "\\#SPILL!"。但对于此类情况，我们仍返回该公式应溢出的整个范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arrayFormula | java.lang.String | 公式表达式 |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。\"Parse\" 选项将被忽略，公式将始终立即解析 |
| 值 | java.lang.Object[][] | values（计算结果）用于具有给定动态数组公式的单元格 |
| calculateRange | boolean | 是否计算此动态数组公式的溢出范围。如果 \"values\" 参数不为 null 且此标志为 false，则溢出范围的高度将为 values.Length，宽度将为 values[0].Length。 |
| calculateValue | boolean | 当 \"values\" 为 null 或某单元格对应的 \"values\" 项为 null 时，是否为溢出范围内的单元格计算此动态数组公式。 |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```


设置动态数组公式，并在可能的情况下使公式溢出到相邻单元格。

**Remarks**

返回的范围可能与此动态数组公式实际溢出的范围不同。如果范围内有非空单元格，公式将仅设置在当前单元格并标记为 "\\#SPILL!"。但对于此类情况，我们仍返回该公式应溢出的整个范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arrayFormula | java.lang.String | 公式表达式 |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。\"Parse\" 选项将被忽略，公式将始终立即解析 |
| 值 | java.lang.Object[][] | values（计算结果）用于具有给定动态数组公式的单元格 |
| calculateRange | boolean | 是否计算此动态数组公式的溢出范围。如果 \"values\" 参数不为 null 且此标志为 false，则溢出范围的高度将为 values.Length，宽度将为 values[0].Length。 |
| calculateValue | boolean | 当 \"values\" 为 null 或某单元格对应的 \"values\" 项为 null 时，是否为溢出范围内的单元格计算此动态数组公式。 |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 用于计算公式的选项。通常出于性能考虑，[CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\\#getRecursive--) 属性应为 false。 |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```


设置单元格中的嵌入图像。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


设置 [Cell](../../com.aspose.cells/cell) 的公式。

**Remarks**

公式字符串总是以等号 (=) 开头。并请始终使用逗号 (,) 作为参数分隔符，例如 "=SUM(A1, E1, H2)"。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```


设置公式及公式的值。

**Remarks**

注意：此类已过时。请改用 Cell.SetFormula(string,FormulaParseOptions,object)。此属性将在自 2019 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 公式。 |
| isR1C1 | boolean | 公式是否为 R1C1 公式。 |
| isLocal | boolean | 公式是否已本地化格式化。 |
| 值 | java.lang.Object | 公式的值。 |

### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```


设置公式及公式的值（计算结果）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 公式。 |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。 |

### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```


设置公式及公式的值（计算结果）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 公式。 |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。 |
| 值 | java.lang.Object | 公式的值（计算结果）。 |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


设置公式及公式的值（计算结果）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 公式。 |
| 值 | java.lang.Object | 公式的值（计算结果）。 |

### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```


获取单元格的本地化格式公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


设置包含数据和某些格式的 HTML 字符串到此单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```


设置 [Cell](../../com.aspose.cells/cell) 的 R1C1 公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```


为一系列单元格设置共享公式。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sharedFormula | java.lang.String | 共享公式。 |
| rowNumber | int | 用于填充公式的行数。 |
| columnNumber | int | 用于填充公式的列数。 |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


为一系列单元格设置公式。

**Remarks**

注意：此类已过时。请改用 Cell.SetSharedFormula(string,int,int,FormulaParseOptions)。此属性将在自 2019 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sharedFormula | java.lang.String | 共享公式。 |
| rowNumber | int | 用于填充公式的行数。 |
| columnNumber | int | 用于填充公式的列数。 |
| isR1C1 | boolean | 公式是否为 R1C1 公式 |
| isLocal | boolean | 公式是否为本地化格式 |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


为一系列单元格设置共享公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sharedFormula | java.lang.String | 共享公式。 |
| rowNumber | int | 用于填充公式的行数。 |
| columnNumber | int | 用于填充公式的列数。 |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。 |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


为一系列单元格设置共享公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sharedFormula | java.lang.String | 共享公式。 |
| rowNumber | int | 用于填充公式的行数。 |
| columnNumber | int | 用于填充公式的列数。 |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。 |
| 值 | java.lang.Object[][] | values 用于具有给定共享公式的单元格 |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


设置单元格样式。

**Remarks**

如果更改了边框设置，调整单元格的边框也会相应更新。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 单元格样式。 |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


将样式的已更改属性应用到单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 单元格样式。 |
| explicitFlag | boolean | True，仅覆盖已显式设置的格式。 |

### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```


根据标志应用单元格样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 单元格样式。 |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | 样式标志。 |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```


从此单元格开始，为给定范围创建单变量数据表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowNumber | int | 用于填充公式的行数。 |
| columnNumber | int | 用于填充公式的列数。 |
| rowIndexOfInputCell | int | 输入单元格的行索引 |
| columnIndexOfInputCell | int | 输入单元格的列索引 |
| isRowInput | boolean | 指示输入单元格是行输入单元格（true）还是列输入单元格（false）。 |
| 值 | java.lang.Object[][] | 表格公式范围内单元格的值 |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```


从此单元格开始，为给定范围创建双变量数据表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowNumber | int | 用于填充公式的行数。 |
| columnNumber | int | 用于填充公式的列数。 |
| rowIndexOfRowInputCell | int | 行输入单元格的行索引 |
| columnIndexOfRowInputCell | int | 行输入单元格的列索引 |
| rowIndexOfColumnInputCell | int | 列输入单元格的行索引 |
| columnIndexOfColumnInputCell | int | 列输入单元格的列索引 |
| 值 | java.lang.Object[][] | 表格公式范围内单元格的值 |

### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```


从此单元格开始，为给定范围创建单变量数据表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowNumber | int | 用于填充公式的行数。 |
| columnNumber | int | 用于填充公式的列数。 |
| inputCell | java.lang.String | 输入单元格 |
| isRowInput | boolean | 指示输入单元格是行输入单元格（true）还是列输入单元格（false）。 |
| 值 | java.lang.Object[][] | 表格公式范围内单元格的值 |

### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```


从此单元格开始，为给定范围创建双变量数据表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowNumber | int | 用于填充公式的行数。 |
| columnNumber | int | 用于填充公式的列数。 |
| rowInputCell | java.lang.String | 行输入单元格 |
| columnInputCell | java.lang.String | 列输入单元格 |
| 值 | java.lang.Object[][] | 表格公式范围内单元格的值 |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


设置此单元格中包含的值。

**Remarks**

可能的类型：

null，

Boolean，

DateTime，

Double，

Integer

String。

对于 int 值，可能返回 Integer 对象或 Double 对象。且无法保证返回的值始终保持相同的对象类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### toJson() {#toJson--}
```
public String toJson()
```


将 [Cell](../../com.aspose.cells/cell) 转换为 JSON 结构数据。

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


返回表示当前 Cell 对象的字符串。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

