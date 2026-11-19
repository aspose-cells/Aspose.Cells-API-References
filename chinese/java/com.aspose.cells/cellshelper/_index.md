---
title: "CellsHelper"
second_title: "Aspose.Cells for Java API 参考"
description: "提供辅助函数。"
type: docs
url: /zh/java/com.aspose.cells/cellshelper/
---

**Inheritance:**
java.lang.Object
```
public class CellsHelper
```

提供辅助函数。
## 方法

| 方法 | 描述 |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | 添加插件功能。 |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | 根据行列索引获取单元格名称。 |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | 根据单元格名称获取其行列索引。 |
| [columnIndexToName(int column)](#columnIndexToName-int-) | 根据列索引获取列名称。 |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | 根据列名称获取列索引。 |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | 将单元格的 A1 公式转换为 r1c1 公式。 |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | 将单元格的 r1c1 公式转换为 A1 公式。 |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | 检查给定的工作表名称，并在需要时创建有效的名称。 |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | 检查给定的工作表名称，并在需要时创建有效的名称。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | 获取备用启动路径，该路径被某些外部公式引用。 |
| [getCacheFolder()](#getCacheFolder--) | 获取用于临时文件的文件夹，这些文件可能用作数据缓存。 |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | 获取用于创建具有特殊实现的实例的工厂。 |
| [getDPI()](#getDPI--) | 获取机器的 DPI。 |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | 将 double 值转换为日期时间值。 |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | 将日期时间转换为 double 值。 |
| [getLibraryPath()](#getLibraryPath--) | 获取某些外部公式引用所指的库路径。 |
| [getSignificantDigits()](#getSignificantDigits--) | 获取有效数字的位数。 |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | 获取用于输出数值的默认有效数字类型。 |
| [getStartupPath()](#getStartupPath--) | 获取启动路径，该路径被某些外部公式引用。 |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | 获取文本的宽度（单位为点）。 |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | 获取工作簿中使用的所有颜色。 |
| [getVersion()](#getVersion--) | 获取发布版本。 |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | 请在云平台上运行时将此属性设置为 True，例如：Azure、AWSLambda 等， |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | 将一些大型 xls 文件合并为一个 xls 文件。 |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | 指示工作表名称是否应被单引号括起 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | 根据行索引获取行名。 |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | 根据行名获取行索引。 |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | 设置备用启动路径，该路径被某些外部公式引用。 |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | 设置可能用作数据缓存的临时文件夹。 |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | 请在云平台上运行时将此属性设置为 True，例如：Azure、AWSLambda 等， |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | 设置用于创建具有特殊实现的实例的工厂。 |
| [setDPI(double value)](#setDPI-double-) | 获取机器的 DPI。 |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | 设置某些外部公式引用所指的库路径。 |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | 设置有效数字的位数。 |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | 设置用于输出数值的默认有效数字类型。 |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | 设置启动路径，该路径被某些外部公式引用。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```


添加插件功能。

**Remarks**

注意：此成员现已过时。请改用 WorksheetCollection.RegisterAddInFunction() 方法。该方法将在自 2022 年 1 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 函数 | java.lang.String | 函数名称。 |
| minCountOfParameters | int | 此函数所需的最小参数数量 |
| maxCountOfParameters | int | 此函数允许的最大参数数量。 |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype)。该函数的预期参数类型 |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype)。函数的返回值类型 |

### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


根据行列索引获取单元格名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 单元格名称。
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```


根据单元格名称获取其行列索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称 |

**Returns:**
int[] - [0] 为行索引，[1] 为列索引。
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


根据列索引获取列名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 列名称。
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


根据列名称获取列索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnName | java.lang.String | 列名称。 |

**Returns:**
int - 列索引。
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```


将单元格的 A1 公式转换为 r1c1 公式。

**Remarks**

注意：此成员已过时。请改用 Worksheet.ConvertFormulaReferenceStyle() 方法。自2023年8月起，此属性将在12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | A1 公式。 |
| 行 | int | 单元格的行索引。 |
| 列 | int | 单元格的列索引。 |

**Returns:**
java.lang.String - R1C1 公式。
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```


将单元格的 r1c1 公式转换为 A1 公式。

**Remarks**

注意：此成员已过时。请改用 Worksheet.ConvertFormulaReferenceStyle() 方法。自2023年8月起，此属性将在12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| r1c1Formula | java.lang.String | r1c1 公式。 |
| 行 | int | 单元格的行索引。 |
| 列 | int | 单元格的列索引。 |

**Returns:**
java.lang.String - A1 公式。
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```


检查给定的工作表名称，并在需要时创建有效名称。如果给定的工作表名称符合 Excel 工作表名称规则，则返回该名称。否则，当长度超出限制时，字符串将被截断，且无效字符将被替换为' '，随后返回重建后的字符串值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| nameProposal | java.lang.String | 要使用的工作表名称 |

**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```


检查给定的工作表名称，并在需要时创建一个有效的名称。如果给定的工作表名称符合 Excel 工作表名称的规则，则返回它。否则，如果长度超过限制，字符串将被截断，且无效字符将被替换为给定字符，然后返回重建后的字符串值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| nameProposal | java.lang.String | 要使用的工作表名称 |
| replaceChar | char | 用于替换给定工作表名称中无效字符的字符 |

**Returns:**
java.lang.String -
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```


获取备用启动路径，该路径被某些外部公式引用。

**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```


获取用于临时文件的文件夹，这些文件可能用作数据缓存。

**Remarks**

缓存文件通常用于某些功能以考虑内存性能，例如将大型数据集保存为 xls 文件，或在单元格模型中使用带文件缓存的内存模式。

**Returns:**
java.lang.String - 已指定的缓存文件文件夹。如果未指定，将返回 null，并在需要时使用系统的临时路径。
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```


获取用于创建具有特殊实现的实例的工厂。

**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```


获取机器的 DPI。

**Remarks**

**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```


将 double 值转换为日期时间值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| doubleValue | double | 双精度值。 |
| date1904 | boolean | 1904 日期系统。 |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - 
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```


将日期时间转换为 double 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | 日期时间。 |
| date1904 | boolean | 1904 日期系统。 |

**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```


获取某些外部公式引用所指的库路径。

**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```


获取有效数字的位数。默认值为 17。

**Remarks**

现在只能是 15 或 17。注意：此成员已过时。请改用 [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--)。此属性将在自 2025 年 6 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```


获取用于输出数值的默认有效数字类型。默认值为 [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17)。

参见 [SignificantDigitsType](../../com.aspose.cells/significantdigitstype)。

**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```


获取启动路径，该路径被某些外部公式引用。

**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```


获取文本的宽度（单位为点）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | java.lang.String | 文本。 |
| font | [Font](../../com.aspose.cells/font) | 文本的字体。 |
| scaling | double | 文本的缩放。 |

**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```


获取工作簿中使用的所有颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | 工作簿对象。 |

**Returns:**
com.aspose.cells.Color[] - 使用的颜色。
### getVersion() {#getVersion--}
```
public static String getVersion()
```


获取发布版本。

**Returns:**
java.lang.String - 发布版本。
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```


请在云平台上运行时将此属性设置为 True，例如：Azure、AWSLambda 等，

**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```


将一些大型 xls 文件合并为一个 xls 文件。

**Remarks**

此方法仅支持将数据、样式和公式合并到新文件。缓存文件用于存储一些临时数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件 | java.lang.String[] | 这些文件。 |
| cachedFile | java.lang.String | 缓存的文件。 |
| destFile | java.lang.String | 目标文件。 |

### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```


指示工作表名称是否应被单引号括起

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 工作表的名称 |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```


根据行索引获取行名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |

**Returns:**
java.lang.String - 行的名称。
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```


根据行名获取行索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowName | java.lang.String | 行名称。 |

**Returns:**
int - 行索引。
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```


设置备用启动路径，该路径被某些外部公式引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```


设置可能用作数据缓存的临时文件夹。

**Remarks**

缓存文件通常用于某些功能以考虑内存性能，例如将大型数据集保存为 xls 文件，或在单元格模型中使用带文件缓存的内存模式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cache | java.lang.String | 用于临时文件的文件夹，这些文件可能用作数据缓存。 |

### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```


请在云平台上运行时将此属性设置为 True，例如：Azure、AWSLambda 等，

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```


设置用于创建具有特殊实现的实例的工厂。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


获取机器的 DPI。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```


设置某些外部公式引用所指的库路径。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```


设置有效数字的位数。默认值为 17。

**Remarks**

现在只能是 15 或 17。注意：此成员已过时。请改用 [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--)。此属性将在自 2025 年 6 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```


设置输出数值时的默认有效数字类型。默认值为 [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17)。

参见 [SignificantDigitsType](../../com.aspose.cells/significantdigitstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```


设置启动路径，该路径被某些外部公式引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

