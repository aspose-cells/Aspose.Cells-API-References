---
title: "Workbook"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于创建 Excel 电子表格的根对象。"
type: docs
url: /zh/java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

表示用于创建 Excel 电子表格的根对象。

**Remarks**

Workbook 类表示一个 Excel 电子表格。每个电子表格可以包含多个工作表。该类的基本功能是打开和保存本机 Excel 文件。该类还具有一些高级功能，例如从其他 Workbook 复制数据、合并两个 Workbook、将 Excel 转换为 PDF、将 Excel 渲染为图像以及保护 Excel 电子表格。

**Example**

以下示例从名为 designer.xls 的 Excel 文件加载一个 Workbook，并使水平和垂直滚动条不可见。随后在电子表格中将两个字符串值分别替换为整数值和字符串值，最后将工作簿保存为 Excel xlsx 文件。

```
         //Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xlsx");
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Workbook()](#Workbook--) | 初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例。 |
| [Workbook(int fileFormatType)](#Workbook-int-) | 初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例。 |
| [Workbook(LoadOptions loadOptions)](#Workbook-com.aspose.cells.LoadOptions-) | 使用选项初始化一个新的空的 [Workbook](../../com.aspose.cells/workbook) 类实例 |
| [Workbook(String file)](#Workbook-java.lang.String-) | 初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例并打开文件。 |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | 初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例并打开流。 |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | 初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例并打开文件。 |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | 初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例并打开流。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | 接受工作簿中所有已跟踪的更改。 |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | 向 OOXML 电子表格文件（Excel2007 及更高版本）添加数字签名。 |
| [calculateFormula()](#calculateFormula--) | 计算公式的结果。 |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | 计算公式的结果。 |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | 正在计算此工作簿中的公式。 |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | 更改指定索引处的电子表格调色板。 |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | 关闭使用缓存访问数据的会话。 |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | 合并另一个 Workbook 对象。 |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | 从源 Workbook 对象复制数据。 |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | 复制另一个 Workbook 对象。 |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | 从另一本工作簿复制主题。 |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | 根据给定类型创建内置样式。 |
| [createCellsColor()](#createCellsColor--) | 创建一个 [CellsColor](../../com.aspose.cells/cellscolor) 对象。 |
| [createStyle()](#createStyle--) | 创建新样式。 |
| [createStyle(boolean cloneDefaultStyle)](#createStyle-boolean-) | 创建新样式。 |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | 自定义主题。 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | 导出由指定 XML 映射链接的 XML 数据。 |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | 导出由指定 XML 映射链接的 XML 数据。 |
| [getAbsolutePath()](#getAbsolutePath--) | 获取文件的绝对路径。 |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | 返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有内置文档属性。 |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | 获取用于从自定义对象构建 ICellsDataTable 的工厂 |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | 返回电子表格调色板中的颜色。 |
| [getContentTypeProperties()](#getContentTypeProperties--) | 获取工作簿中 [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) 对象的列表。 |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | 获取样式池中样式的数量。 |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | 返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有自定义文档属性。 |
| [getCustomXmlParts()](#getCustomXmlParts--) | 表示自定义 XML 数据存储部件（包内的自定义 XML 数据）。 |
| [getDataConnections()](#getDataConnections--) | 获取 [ExternalConnection](../../com.aspose.cells/externalconnection) 集合。 |
| [getDataMashup()](#getDataMashup--) | 获取 mashup 数据。 |
| [getDataModel()](#getDataModel--) | 获取工作簿中的数据模型。 |
| [getDataSorter()](#getDataSorter--) | 获取用于排序数据的 DataSorter 对象。 |
| [getDefaultStyle()](#getDefaultStyle--) | 获取工作簿的默认 [Style](../../com.aspose.cells/style) 对象。 |
| [getDigitalSignature()](#getDigitalSignature--) | 从文件获取数字签名。 |
| [getFileFormat()](#getFileFormat--) | 获取文件格式。 |
| [getFileName()](#getFileName--) | 获取当前文件名。 |
| [getFonts()](#getFonts--) | 获取样式池中的所有字体。 |
| [getInterruptMonitor()](#getInterruptMonitor--) | 获取中断监视器。 |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | 在当前调色板中查找最匹配的颜色。 |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | 获取样式池中命名的样式。 |
| [getRibbonXml()](#getRibbonXml--) | 获取定义 Ribbon UI 的 XML 文件。 |
| [getSettings()](#getSettings--) | 表示工作簿设置。 |
| [getStyleInPool(int index)](#getStyleInPool-int-) | 获取样式池中的样式。 |
| [getTheme()](#getTheme--) | 获取主题名称。 |
| [getThemeColor(int type)](#getThemeColor-int-) | 获取主题颜色。 |
| [getVbaProject()](#getVbaProject--) | 获取电子表格中的 [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--)。 |
| [getWorksheets()](#getWorksheets--) | 获取电子表格中的 [WorksheetCollection](../../com.aspose.cells/worksheetcollection) 集合。 |
| [hasCustomFunction()](#hasCustomFunction--) | 检测此工作簿中是否使用了自定义函数，例如在单元格公式或已定义名称中…… |
| [hasExernalLinks()](#hasExernalLinks--) | 指示此工作簿是否包含指向其他数据源的外部链接。 |
| [hasMacro()](#hasMacro--) | 指示此电子表格是否包含宏/VBA。 |
| [hasRevisions()](#hasRevisions--) | 获取工作簿是否有任何已跟踪的更改 |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | 将 XML 数据文件导入/更新到工作簿中。 |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | 将 XML 数据文件导入/更新到工作簿中。 |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | 检查颜色是否在电子表格的调色板中。 |
| [isDigitallySigned()](#isDigitallySigned--) | 指示此电子表格是否已数字签名。 |
| [isLicensed()](#isLicensed--) | 指示是否已设置许可证。 |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | 指示结构或窗口是否已使用密码受保护。 |
| [mergeNamedStyles(Workbook source)](#mergeNamedStyles-com.aspose.cells.Workbook-) | 合并来自其他 Excel 文件的命名样式。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | 解析所有在从模板文件加载或设置到单元格时未被解析的公式。 |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | 保护工作簿。 |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | 保护共享工作簿。 |
| [refreshAll()](#refreshAll--) | 刷新链接的形状、所有数据透视表和带有数据透视源的图表。 |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | 刷新动态数组公式（根据当前数据溢出到相邻单元格的新范围），工作簿中的其他公式即使被动态数组公式使用也不会递归计算。 |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | 刷新动态数组公式（根据当前数据溢出到相邻单元格的新范围） |
| [removeDigitalSignature()](#removeDigitalSignature--) | 从此电子表格中移除数字签名。 |
| [removeExternalLinks()](#removeExternalLinks--) | 移除工作簿中的所有外部链接。 |
| [removeMacro()](#removeMacro--) | 从此电子表格中移除 VBA/宏。 |
| [removePersonalInformation()](#removePersonalInformation--) | 移除个人信息。 |
| [removeUnusedStyles()](#removeUnusedStyles--) | 移除所有未使用的样式。 |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | 将单元格的值替换为新数据。 |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | 将单元格的值替换为新数据。 |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | 将单元格的值替换为新的 double。 |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | 将单元格的值替换为 double 数组。 |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | 将单元格的值替换为新的 integer。 |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | 将单元格的值替换为 integer 数组。 |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | 将单元格的值替换为新的 string。 |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | 将单元格的值替换为新的 string。 |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | 将单元格的值替换为新的 string 数组。 |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | 将工作簿保存到流中。 |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | 将工作簿保存到流中。 |
| [save(String fileName)](#save-java.lang.String-) | 将工作簿保存到磁盘。 |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | 将工作簿保存到磁盘。 |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | 将工作簿保存到磁盘。 |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | 设置文件的绝对路径。 |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | 设置工作簿的默认 [Style](../../com.aspose.cells/style) 对象。 |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | 为电子表格文件（Excel2007 及更高版本）设置数字签名。 |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | 设置加密选项。 |
| [setFileFormat(int value)](#setFileFormat-int-) | 设置文件格式。 |
| [setFileName(String value)](#setFileName-java.lang.String-) | 设置当前文件名。 |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | 设置中断监视器。 |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | 设置定义 Ribbon UI 的 XML 文件。 |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | 设置主题颜色 |
| [startAccessCache(int opts)](#startAccessCache-int-) | 启动使用缓存访问数据的会话。 |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | 取消对工作簿的保护。 |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | 取消对共享工作簿的保护。 |
| [updateCustomFunctionDefinition(CustomFunctionDefinition definition)](#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | 更新自定义函数的定义。 |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | 如果此工作簿包含指向其他数据源的外部链接，Aspose.Cells 将尝试从给定的源检索最新数据。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例。

**Remarks**

默认文件格式类型是 Xlsx。如果您想创建其他类型的文件，请使用 Workbook(FileFormatType)。

**Example**

以下代码展示了如何使用 Workbook 构造函数来创建并初始化该类的新实例。

```
         Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例。

**Remarks**

默认文件格式类型是 Excel97To2003。

**Example**

以下代码展示了如何使用 Workbook 构造函数创建并初始化类的一个新实例，使用各种文件格式类型。

```
         Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileFormatType | int | [FileFormatType](../../com.aspose.cells/fileformattype). 新的文件格式。 |

### Workbook(LoadOptions loadOptions) {#Workbook-com.aspose.cells.LoadOptions-}
```
public Workbook(LoadOptions loadOptions)
```


使用选项初始化一个新的空的 [Workbook](../../com.aspose.cells/workbook) 类实例

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | 选项。 |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例并打开文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件 | java.lang.String | 文件名。 |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例并打开流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | 该流。 |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例并打开文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件 | java.lang.String | 文件名。 |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | 加载选项 |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


初始化一个新的 [Workbook](../../com.aspose.cells/workbook) 类实例并打开流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | 该流。 |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | 加载选项 |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


接受工作簿中所有已跟踪的更改。

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


向 OOXML 电子表格文件（Excel2007 及更高版本）添加数字签名。

**Remarks**

仅支持向 OOXML 电子表格文件添加 Xmldsig 数字签名

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


计算公式的结果。

**Remarks**

有关所有受支持的公式，请查看 https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions 上的列表。

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


计算公式的结果。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ignoreError | boolean | 指示是否隐藏公式计算中的错误。错误可能是未受支持的函数、外部链接等。 |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


正在计算此工作簿中的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 计算的选项 |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


更改指定索引处的电子表格调色板。

**Remarks**

调色板有 56 个条目，每个条目由 RGB 值表示。

如果设置的颜色不在调色板中，则不会生效。

因此，如果您想设置自定义颜色，请先更改调色板。

以下是标准颜色调色板。

| Color | 红色 | 绿色 | 蓝色 |
| ------- | --- | ----- | ---- |
| 黑色 | 0 | 0 | 0 |
| 白色 | 255 | 255 | 255 |
| 红色 | 255 | 0 | 0 |
| 青柠色 | 0 | 255 | 0 |
| 蓝色 | 0 | 0 | 255 |
| 黄色 | 255 | 255 | 0 |
| 品红色 | 255 | 0 | 255 |
| 青色 | 0 | 255 | 255 |
| 栗色 | 128 | 0 | 0 |
| 绿色 | 0 | 128 | 0 |
| 海军蓝 | 0 | 0 | 128 |
| 橄榄绿 | 128 | 128 | 0 |
| 紫色 | 128 | 0 | 128 |
| 青色 | 0 | 128 | 128 |
| 银色 | 192 | 192 | 192 |
| 灰色 | 128 | 128 | 128 |
| 颜色17 | 153 | 153 | 255 |
| 颜色18 | 153 | 51 | 102 |
| 颜色19 | 255 | 255 | 204 |
| 颜色20 | 204 | 255 | 255 |
| 颜色21 | 102 | 0 | 102 |
| 颜色22 | 255 | 128 | 128 |
| 颜色23 | 0 | 102 | 204 |
| 颜色24 | 204 | 204 | 255 |
| 颜色25 | 0 | 0 | 128 |
| 颜色26 | 255 | 0 | 255 |
| 颜色27 | 255 | 255 | 0 |
| 颜色28 | 0 | 255 | 255 |
| 颜色29 | 128 | 0 | 128 |
| 颜色30 | 128 | 0 | 0 |
| 颜色31 | 0 | 128 | 128 |
| 颜色32 | 0 | 0 | 255 |
| 颜色33 | 0 | 204 | 255 |
| 颜色34 | 204 | 255 | 255 |
| 颜色35 | 204 | 255 | 204 |
| 颜色36 | 255 | 255 | 153 |
| 颜色37 | 153 | 204 | 255 |
| 颜色38 | 255 | 153 | 204 |
| 颜色39 | 204 | 153 | 255 |
| 颜色40 | 255 | 204 | 153 |
| 颜色41 | 51 | 102 | 255 |
| 颜色42 | 51 | 204 | 204 |
| 颜色43 | 153 | 204 | 0 |
| 颜色44 | 255 | 204 | 0 |
| 颜色45 | 255 | 153 | 0 |
| 颜色46 | 255 | 102 | 0 |
| 颜色47 | 102 | 102 | 153 |
| 颜色48 | 150 | 150 | 150 |
| 颜色49 | 0 | 51 | 102 |
| 颜色50 | 51 | 153 | 102 |
| 颜色51 | 0 | 51 | 0 |
| 颜色52 | 51 | 51 | 0 |
| 颜色53 | 153 | 51 | 0 |
| 颜色54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | 颜色结构。 |
| 索引 | int | 调色板索引，0 - 55。 |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


关闭使用缓存访问数据的会话。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). 数据访问的选项 |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


合并另一个 Workbook 对象。

**Remarks**

将 Excel、ODS、CSV 和其他文件合并为一个文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | 另一个 Workbook 对象。 |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


从源 Workbook 对象复制数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | 源 Workbook 对象。 |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


复制另一个 Workbook 对象。

**Remarks**

克隆 Excel 文件非常简单。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | 源 Workbook 对象。 |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | 复制其他工作簿的选项。 |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


从另一本工作簿复制主题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | 源工作簿。 |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


根据给定类型创建内置样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [BuiltinStyleType](../../com.aspose.cells/builtinstyletype). 内置样式类型。 |

**Returns:**
[Style](../../com.aspose.cells/style) - [Style](../../com.aspose.cells/style) object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


创建一个 [CellsColor](../../com.aspose.cells/cellscolor) 对象。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


创建新样式。

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### createStyle(boolean cloneDefaultStyle) {#createStyle-boolean-}
```
public Style createStyle(boolean cloneDefaultStyle)
```


创建新样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cloneDefaultStyle | boolean | 指示是否克隆默认样式 |

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


自定义主题。

**Remarks**

颜色的长度应为 12。

| 数组索引 | 主题类型 |
| ----------- | ------------------ |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Backgournd2 |
| 3 | Text2 |
| 4 | Accent1 |
| 5 | Accent2 |
| 6 | Accent3 |
| 7 | Accent4 |
| 8 | Accent5 |
| 9 | Accent6 |
| 10 | 超链接 |
| 11 | 已访问的超链接 |

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| themeName | java.lang.String | 主题名称 |
| colors | [Color\[\]](../../com.aspose.cells/color) | 主题颜色 |

### dispose() {#dispose--}
```
public void dispose()
```


执行应用程序定义的任务，以释放、释放或重置非托管资源。

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


导出由指定 XML 映射链接的 XML 数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| mapName | java.lang.String | 需要导出的 XML 映射的名称 |
| stream | java.io.OutputStream | 导出流 |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


导出由指定 XML 映射链接的 XML 数据。

**Example**

以下代码导出了第一个 XmlMap 链接的数据。

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| mapName | java.lang.String | 需要导出的 XML 映射的名称 |
| 路径 | java.lang.String | 导出路径 |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


获取文件的绝对路径。

**Remarks**

仅用于外部链接。

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有内置文档属性。

**Remarks**

不能向内置文档属性列表添加新属性。只能获取内置属性并更改其值。以下是内置属性名称列表:

标题

主题

作者

关键字

注释

模板

最后作者

修订号

应用程序名称

最后打印日期

创建日期

最后保存时间

总编辑时间

页数

单词数

字符数

安全性

类别

格式

管理员

公司

字节数

行数

段落数

幻灯片数

备注数

隐藏幻灯片数

多媒体剪辑数

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


获取用于从自定义对象构建 ICellsDataTable 的工厂

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


返回电子表格调色板中的颜色。

**Remarks**

调色板有 56 个条目，每个条目由 RGB 值表示。

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


获取工作簿中 [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) 对象的列表。

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


获取样式池中样式的数量。

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有自定义文档属性。

**Example**

```
         Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


表示自定义 XML 数据存储部件（包内的自定义 XML 数据）。

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


获取 [ExternalConnection](../../com.aspose.cells/externalconnection) 集合。

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


获取 mashup 数据。

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataModel() {#getDataModel--}
```
public DataModel getDataModel()
```


获取工作簿中的数据模型。

**Returns:**
[DataModel](../../com.aspose.cells/datamodel)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


获取用于排序数据的 DataSorter 对象。

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


获取工作簿的默认 [Style](../../com.aspose.cells/style) 对象。

**Remarks**

DefaultStyle 属性对于为整个工作簿实现样式很有用。

**Example**

以下代码创建并实例化一个新的 Workbook，并为其设置默认的 [Style](../../com.aspose.cells/style)。

```
         Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


从文件获取数字签名。

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


获取文件格式。

请参阅 [FileFormatType](../../com.aspose.cells/fileformattype)。

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


获取当前文件名。

**Remarks**

如果文件是通过流打开且存在一些外部公式引用，请设置文件名。

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


获取样式池中的所有字体。

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


获取中断监视器。

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


在当前调色板中查找最匹配的颜色。

**Remarks**

Excel 97-2003 的颜色调色板中只有 56 种颜色。如果颜色不在调色板中，将设置相似的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | 原始颜色。 |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


获取样式池中命名的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 样式名称 |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


获取定义 Ribbon UI 的 XML 文件。

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


表示工作簿设置。

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


获取样式池中的样式。工作簿中的所有样式将被收集到一个池中。单元格中只有一个简单的引用索引。

**Remarks**

如果返回的样式被更改，所有单元格（引用此样式的）样式也将被更改。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


获取主题名称。

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


获取主题颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype)。主题颜色类型。 |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


获取电子表格中的 [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--)。

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


获取电子表格中的 [WorksheetCollection](../../com.aspose.cells/worksheetcollection) 集合。

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


检测此工作簿中是否使用了自定义函数，例如在单元格公式或已定义名称中……

**Returns:**
boolean
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


指示此工作簿是否包含指向其他数据源的外部链接。

**Remarks**

注意：此成员已过时。请改用 ExternalLinkCollection.Count 来检查此工作簿中是否存在外部链接。此方法将在自 2021 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
布尔值 - 此工作簿是否包含指向其他数据源的外部链接。
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


指示此电子表格是否包含宏/VBA。

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


获取工作簿是否有任何已跟踪的更改

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


将 XML 数据文件导入/更新到工作簿中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | XML 文件流。 |
| sheetName | java.lang.String | 目标工作表名称。 |
| 行 | int | 目标行。 |
| 列 | int | 目标列。 |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


将 XML 数据文件导入/更新到工作簿中。

**Example**

以下代码将 XML 数据导入工作表 'Sheet 1' 的单元格 A1。

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| URL | java.lang.String | XML 文件的 URL/路径。 |
| sheetName | java.lang.String | 目标工作表名称。 |
| 行 | int | 目标行 |
| 列 | int | 目标列 |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


检查颜色是否在电子表格的调色板中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | 颜色结构。 |

**Returns:**
布尔值 - 如果此颜色在调色板中则返回 true，否则返回 false
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


指示此电子表格是否已数字签名。

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


指示是否已设置许可证。

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


指示结构或窗口是否已使用密码受保护。

**Returns:**
boolean
### mergeNamedStyles(Workbook source) {#mergeNamedStyles-com.aspose.cells.Workbook-}
```
public void mergeNamedStyles(Workbook source)
```


合并来自其他 Excel 文件的命名样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | 另一个文件 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


解析所有在从模板文件加载或设置到单元格时未被解析的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ignoreError | boolean | 是否忽略无效公式的错误。对于单个无效公式，如果忽略错误，则该公式将被忽略，过程将继续解析其他公式；否则将抛出异常。 |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


保护工作簿。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| protectionType | int | [ProtectionType](../../com.aspose.cells/protectiontype). 保护类型。 |
| 密码 | java.lang.String | 用于保护工作簿的密码。 |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


保护共享工作簿。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 密码 | java.lang.String | 用于保护工作簿的密码。 |

### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


刷新链接的形状、所有数据透视表和带有数据透视源的图表。

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


刷新动态数组公式（根据当前数据溢出到相邻单元格的新范围），工作簿中的其他公式即使被动态数组公式使用也不会递归计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 计算 | boolean | 是否计算并更新这些动态数组公式的单元格值 |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


刷新动态数组公式（根据当前数据溢出到相邻单元格的新范围）

**Remarks**

出于性能考虑，当公式本身或其引用的数据发生更改时，我们不会自动刷新所有动态数组公式。因此用户需要在可能影响动态数组公式的操作后手动调用此方法，例如导入/设置单元格值、插入/删除行/列/范围，等等。

对于大多数带函数的公式，计算溢出范围也需要计算公式，因此通常建议将 "calculate" 标志设为 true。如果公式很简单，例如范围引用或数组（例如 "=C1:E5"、"=\\{1,2;3,4\\}"，...），对范围或数组的简单函数（例如 "=ABS(C1:E5)"、"=1+\\{1,2;3,4\\}"，...），并且所有公式将在稍后计算（例如通过 [calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\\#calculateFormula-CalculationOptions-)），则将 "calculate" 标志设为 false 可以避免重复计算，从而提升性能。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 计算 | boolean | 是否计算并更新这些动态数组公式的单元格值 |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 计算公式的选项 |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


从此电子表格中移除数字签名。

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


移除工作簿中的所有外部链接。

**Remarks**

注意：此成员已过时。请改用 ExternalLinkCollection.Clear() 方法。该方法将在自 2021 年12月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


从此电子表格中移除 VBA/宏。

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


移除个人信息。

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


移除所有未使用的样式。

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


将单元格的值替换为新数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| boolValue | boolean | 要替换的布尔值。 |
| newValue | java.lang.Object | 新值。可以是字符串、整数、双精度或 DateTime 值。 |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


将单元格的值替换为新数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| intValue | int | 要替换的整数值。 |
| newValue | java.lang.Object | 新值。可以是字符串、整数、双精度或 DateTime 值。 |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


将单元格的值替换为新的 double。

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | java.lang.String | 单元格占位符 |
| newValue | double | 要替换的双精度值 |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


将单元格的值替换为 double 数组。

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | java.lang.String | 单元格占位符 |
| newValues | double[] | 要替换的双精度数组 |
| isVertical | boolean | True - 垂直，False - 水平 |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


将单元格的值替换为新的 integer。

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | java.lang.String | 单元格占位符 |
| newValue | int | 要替换的整数值 |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


将单元格的值替换为 integer 数组。

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | java.lang.String | 单元格占位符 |
| newValues | int[] | 要替换的整数数组 |
| isVertical | boolean | True - 垂直，False - 水平 |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


将单元格的值替换为新的 string。

**Example**

```
         Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | java.lang.String | 单元格占位符 |
| newValue | java.lang.String | 要替换的字符串值 |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


将单元格的值替换为新的 string。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | java.lang.String | 单元格占位符 |
| newValue | java.lang.String | 要替换的字符串值 |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | 替换选项 |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


将单元格的值替换为新的 string 数组。

**Example**

```
         Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | java.lang.String | 单元格占位符 |
| newValues | java.lang.String[] | 要替换的字符串数组 |
| isVertical | boolean | True - 垂直，False - 水平 |

**Returns:**
int
### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


将工作簿保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 文件流。 |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | 保存选项。 |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


将工作簿保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 文件流。 |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat)。保存文件格式类型。 |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


将工作簿保存到磁盘。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


将工作簿保存到磁盘。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 文件名。 |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | 保存选项。 |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


将工作簿保存到磁盘。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 文件名。 |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat)。保存格式类型。 |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


设置文件的绝对路径。

**Remarks**

仅用于外部链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


设置工作簿的默认 [Style](../../com.aspose.cells/style) 对象。

**Remarks**

DefaultStyle 属性对于为整个工作簿实现样式很有用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


为电子表格文件（Excel2007 及更高版本）设置数字签名。

**Remarks**

仅支持添加 Xmldsig 数字签名

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


设置加密选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| encryptionType | int | [EncryptionType](../../com.aspose.cells/encryptiontype)。加密类型。 |
| keyLength | int | 密钥长度。 |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


设置文件格式。

请参阅 [FileFormatType](../../com.aspose.cells/fileformattype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


设置当前文件名。

**Remarks**

如果文件是通过流打开且存在一些外部公式引用，请设置文件名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


设置中断监视器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


设置定义 Ribbon UI 的 XML 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


设置主题颜色

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype)。主题颜色类型。 |
| color | [Color](../../com.aspose.cells/color) | 主题颜色 |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


启动使用缓存访问数据的会话。

**Remarks**

如果指定数据访问的缓存要求工作表中的某些数据模型为 "只读"，则此工作簿中每个工作表的相应数据模型都将视为 "只读"，用户不应更改它们。

完成数据访问后，应使用相同的选项调用 [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-)，以清除所有缓存并恢复正常访问模式。



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). 数据访问的选项 |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


取消对工作簿的保护。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 密码 | java.lang.String | 用于取消保护工作簿的密码。 |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


取消对共享工作簿的保护。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 密码 | java.lang.String | 用于取消保护工作簿的密码。 |

### updateCustomFunctionDefinition(CustomFunctionDefinition definition) {#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void updateCustomFunctionDefinition(CustomFunctionDefinition definition)
```


更新自定义函数的定义。

**Remarks**

此方法可用于某些特殊场景。例如，如果用户需要对某些自定义函数的参数以数组模式进行计算，则用户可以为这些函数提供实现了 [CustomFunctionDefinition.getArrayModeParameters(String)](../../com.aspose.cells/customfunctiondefinition\#getArrayModeParameters-String-) 的自定义定义。公式数据更新后，在计算相应的自定义函数时，这些指定的参数将自动以数组模式进行计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) | 针对用户特殊需求的自定义函数特殊定义。 |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


如果此工作簿包含指向其他数据源的外部链接，Aspose.Cells 将尝试从给定的源检索最新数据。

**Remarks**

如果找不到对应工作簿的外部链接，则该工作簿将被忽略。因此，当您稍后使用一个新的外部链接设置公式，且希望将被忽略的工作簿链接到该外部链接时，链接将无法执行，直到您再次使用这些工作簿调用此方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | 用于更新此工作簿引用的外部链接数据的工作簿。这些工作簿与外部链接的匹配由 [getFileName()](../../com.aspose.cells/workbook\#getFileName--) 和 [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) 决定。因此，请确保为每个工作簿指定了适当的 [getFileName()](../../com.aspose.cells/workbook\#getFileName--) 值，以便它们能够链接到相应的外部链接。 |

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

