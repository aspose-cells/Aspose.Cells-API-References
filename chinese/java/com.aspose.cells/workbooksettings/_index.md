---
title: "WorkbookSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作簿的所有设置。"
type: docs
url: /zh/java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

表示工作簿的所有设置。

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [dispose()](#dispose--) | 释放资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | 获取文件的作者。 |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | 指定一个布尔值，指示应用程序是否自动压缩工作簿中的图片。 |
| [getAutoRecover()](#getAutoRecover--) | 指示文件是否标记为自动恢复。 |
| [getBuildVersion()](#getBuildVersion--) | 指定应用程序的增量公开发布版本。 |
| [getCheckCompatibility()](#getCheckCompatibility--) | 指示在保存工作簿时是否检查与早期版本的兼容性。 |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | 指示在设置 Style.Custom 时是否检查自定义数字格式。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | 指定输出文档的 OOXML 版本。 |
| [getCrashSave()](#getCrashSave--) | 指示应用程序在崩溃后是否最后一次保存了工作簿文件。 |
| [getDataExtractLoad()](#getDataExtractLoad--) | 指示应用程序是否最后一次打开工作簿以进行数据恢复。 |
| [getDate1904()](#getDate1904--) | 获取一个值，表示工作簿是否使用 1904 日期系统。 |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | 获取图像的默认分辨率。 |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | 获取此工作簿样式相关属性的默认值设置。 |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | 指示是否丢弃编辑的图像数据。 |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | 指示是否以及如何在工作簿中显示对象。 |
| [getEnableMacros()](#getEnableMacros--) | 启用宏； |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | 获取第一个可见的工作表标签。 |
| [getFormulaSettings()](#getFormulaSettings--) | 获取公式相关功能的设置。 |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | 获取全局化设置。 |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | 获取是否隐藏数据透视表的字段列表。 |
| [getLanguageCode()](#getLanguageCode--) | 获取基于已保存文件的 CountryCode 的工作簿版本的用户界面语言。 |
| [getLocale()](#getLocale--) | 获取此工作簿使用的区域设置。 |
| [getMaxColumn()](#getMaxColumn--) | 获取最大列索引（从零开始）。 |
| [getMaxRow()](#getMaxRow--) | 获取最大行索引（从零开始）。 |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | 获取共享公式的最大行号。 |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | 获取每个字段唯一项的限制。 |
| [getMemorySetting()](#getMemorySetting--) | 获取内存使用选项。 |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | 获取用于格式化/解析数值的十进制分隔符。 |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | 获取数值中十进制左侧用于分隔数字组的字符。 |
| [getPaperSize()](#getPaperSize--) | 获取默认打印纸张尺寸。 |
| [getPassword()](#getPassword--) | 表示工作簿文件的加密密码。 |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | 指示此工作簿中所有图表的数据点属性和数据标签是否遵循其引用。 |
| [getProtectionType()](#getProtectionType--) | 获取工作簿的保护类型。 |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | 指示在将以单引号开头的字符串值输入单元格时，是否设置 [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) 属性。 |
| [getRegion()](#getRegion--) | 获取工作簿的区域设置。 |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | 如果可以从指定的工作簿中删除个人信息，则为 True。 |
| [getRepairLoad()](#getRepairLoad--) | 指示应用程序上次是否以安全模式或修复模式打开工作簿。 |
| [getResourceProvider()](#getResourceProvider--) | 获取外部资源的流提供程序，例如加载类型为 "LinkToFile" 的图片的图像数据。 |
| [getShapeDisplayType()](#getShapeDisplayType--) | 获取应用程序在此工作簿中显示形状的方式 |
| [getShared()](#getShared--) | 获取指示工作簿是否共享的值。 |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | 工作表选项卡栏的宽度（以窗口宽度的千分之一为单位）。 |
| [getShowTabs()](#getShowTabs--) | 获取工作簿选项卡是否显示的值。 |
| [getSignificantDigits()](#getSignificantDigits--) | 获取有效数字的位数。 |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | 获取此工作簿中输出数值的有效数字类型。 |
| [getSmartTagOptions()](#getSmartTagOptions--) | 获取智能标签的选项。 |
| [getStreamProvider()](#getStreamProvider--) | 获取外部资源的流提供程序。 |
| [getThemeFont(int type)](#getThemeFont-int-) | 获取默认主题字体名称。 |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | 指示是否更新相邻单元格的边框。 |
| [getUpdateLinksType()](#getUpdateLinksType--) | 获取工作簿打开时如何更新外部链接。 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [getWindowHeight()](#getWindowHeight--) | 窗口的高度，单位为点。 |
| [getWindowHeightCM()](#getWindowHeightCM--) | 窗口的高度，单位为厘米。 |
| [getWindowHeightInch()](#getWindowHeightInch--) | 窗口的高度，单位为英寸。 |
| [getWindowLeft()](#getWindowLeft--) | 从客户端区域左边缘到窗口左边缘的距离，单位为点。 |
| [getWindowLeftCM()](#getWindowLeftCM--) | 从客户端区域左边缘到窗口左边缘的距离。 |
| [getWindowLeftInch()](#getWindowLeftInch--) | 从客户端区域左边缘到窗口左边缘的距离。 |
| [getWindowTop()](#getWindowTop--) | 从客户端区域顶部到窗口顶部的距离，单位为点。 |
| [getWindowTopCM()](#getWindowTopCM--) | 从客户端区域顶部到窗口顶部的距离，单位为厘米。 |
| [getWindowTopInch()](#getWindowTopInch--) | 从客户端区域顶部到窗口顶部的距离，单位为英寸。 |
| [getWindowWidth()](#getWindowWidth--) | 窗口的宽度，单位为点。 |
| [getWindowWidthCM()](#getWindowWidthCM--) | 窗口的宽度，单位为厘米。 |
| [getWindowWidthInch()](#getWindowWidthInch--) | 窗口的宽度，单位为英寸。 |
| [getWpsCompatibility()](#getWpsCompatibility--) | 指示是否兼容 WPS。 |
| [getWriteProtection()](#getWriteProtection--) | 提供对工作簿写保护选项的访问。 |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | 指示在工作簿的结构和窗口被锁定时是否使用默认密码对工作簿进行加密。 |
| [isEncrypted()](#isEncrypted--) | 获取指示是否需要密码才能打开此工作簿的值。 |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | 获取指示生成的电子表格是否包含水平滚动条的值。 |
| [isHidden()](#isHidden--) | 指示此工作簿是否隐藏。 |
| [isMinimized()](#isMinimized--) | 表示生成的电子表格是否以最小化方式打开。 |
| [isProtected()](#isProtected--) | 获取指示工作簿的结构或窗口是否受保护的值。 |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | 获取指示生成的电子表格是否包含垂直滚动条的值。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | 设置文件的作者。 |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | 指定一个布尔值，指示应用程序是否自动压缩工作簿中的图片。 |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | 指示文件是否标记为自动恢复。 |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | 指定应用程序的增量公开发布版本。 |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | 指示在保存工作簿时是否检查与早期版本的兼容性。 |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | 指示在设置 Style.Custom 时是否检查自定义数字格式。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setCompliance(int value)](#setCompliance-int-) | 指定输出文档的 OOXML 版本。 |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | 指示应用程序在崩溃后是否最后一次保存了工作簿文件。 |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | 指示应用程序是否最后一次打开工作簿以进行数据恢复。 |
| [setDate1904(boolean value)](#setDate1904-boolean-) | 设置表示工作簿是否使用 1904 日期系统的值。 |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | 指示在工作簿的结构和窗口被锁定时是否使用默认密码对工作簿进行加密。 |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | 设置图像的默认分辨率。 |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | 指示是否丢弃编辑的图像数据。 |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | 指示是否以及如何在工作簿中显示对象。 |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | 启用宏； |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | 设置第一个可见的工作表标签。 |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | 设置全球化设置。 |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | 设置指示生成的电子表格是否包含水平滚动条的值。 |
| [setHidden(boolean value)](#setHidden-boolean-) | 指示此工作簿是否隐藏。 |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | 设置是否隐藏透视表的字段列表。 |
| [setLanguageCode(int value)](#setLanguageCode-int-) | 根据保存文件的 CountryCode 设置工作簿版本的用户界面语言。 |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | 设置此工作簿使用的区域设置。 |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | 设置共享公式的最大行号。 |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | 设置每个字段的唯一项限制。 |
| [setMemorySetting(int value)](#setMemorySetting-int-) | 设置内存使用选项。 |
| [setMinimized(boolean value)](#setMinimized-boolean-) | 表示生成的电子表格是否以最小化方式打开。 |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | 设置数值格式化/解析的十进制分隔符。 |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | 设置数值中小数点左侧数字分组的分隔字符。 |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | 设置整个工作簿的打印方向类型。 |
| [setPaperSize(int value)](#setPaperSize-int-) | 设置默认打印纸张尺寸。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 表示工作簿文件的加密密码。 |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | 指示此工作簿中所有图表的数据点属性和数据标签是否遵循其引用。 |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | 指示在将以单引号开头的字符串值输入单元格时，是否设置 [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) 属性。 |
| [setRegion(int value)](#setRegion-int-) | 设置工作簿的区域设置。 |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | 如果可以从指定的工作簿中删除个人信息，则为 True。 |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | 指示应用程序上次是否以安全模式或修复模式打开工作簿。 |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | 设置外部资源的流提供程序，例如加载类型为 "LinkToFile" 的图片数据。 |
| [setShapeDisplayType(int value)](#setShapeDisplayType-int-) | 设置应用程序在此工作簿中显示形状的方式 |
| [setShared(boolean value)](#setShared-boolean-) | 设置一个值，指示工作簿是否已共享。 |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | 工作表选项卡栏的宽度（以窗口宽度的千分之一为单位）。 |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | 设置是否显示工作簿标签页的值。 |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | 设置有效数字的位数。 |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | 设置在此工作簿中输出数值时的有效数字类型。 |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | 设置外部资源的流提供程序。 |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | 指示是否更新相邻单元格的边框。 |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | 设置工作簿打开时如何更新外部链接。 |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | 设置一个值，指示生成的电子表格是否包含垂直滚动条。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [setWindowHeight(double value)](#setWindowHeight-double-) | 窗口的高度，单位为点。 |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | 窗口的高度，单位为厘米。 |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | 窗口的高度，单位为英寸。 |
| [setWindowLeft(double value)](#setWindowLeft-double-) | 从客户端区域左边缘到窗口左边缘的距离，单位为点。 |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | 从客户端区域左边缘到窗口左边缘的距离。 |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | 从客户端区域左边缘到窗口左边缘的距离。 |
| [setWindowTop(double value)](#setWindowTop-double-) | 从客户端区域顶部到窗口顶部的距离，单位为点。 |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | 从客户端区域顶部到窗口顶部的距离，单位为厘米。 |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | 从客户端区域顶部到窗口顶部的距离，单位为英寸。 |
| [setWindowWidth(double value)](#setWindowWidth-double-) | 窗口的宽度，单位为点。 |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | 窗口的宽度，单位为厘米。 |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | 窗口的宽度，单位为英寸。 |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | 指示是否兼容 WPS。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


释放资源。

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


获取文件的作者。

**Remarks**

它未设置，请先检查 [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--)，然后检查 Environment 的用户。

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


指定一个布尔值，指示应用程序是否自动压缩工作簿中的图片。

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


指示文件是否标记为自动恢复。

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


指定应用程序的增量公开发布版本。

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


指示在保存工作簿时是否检查与早期版本的兼容性。

**Remarks**

默认值为 true。仅适用于 Excel97-2003 的 xls 或 xlt 文件。

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


指示在设置 Style.Custom 时是否检查自定义数字格式。

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您的输入字符串作为单元格的值，以便稍后能够将完整的字符串值输出为 CSV 等其他文件格式。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式，否则生成的 Excel 文件可能会出现意外错误。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


指定输出文档的 OOXML 版本。默认值为 Ecma376\_2006。

参见 [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance)。

**Remarks**

仅适用于 .xlsx 文件。

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


指示应用程序在崩溃后是否最后一次保存了工作簿文件。

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


指示应用程序是否最后一次打开工作簿以进行数据恢复。

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


获取一个值，表示工作簿是否使用 1904 日期系统。

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


获取图像的默认分辨率。

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


获取此工作簿样式相关属性的默认值设置。

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


指示是否丢弃编辑的图像数据。

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


指示是否以及如何在工作簿中显示对象。

参见 [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects)。

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


启用宏；

**Remarks**

目前仅在将工作表复制到同一工作簿的其他工作表时有效。

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


获取第一个可见的工作表标签。

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


获取公式相关功能的设置。

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


获取全局化设置。

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


获取是否隐藏数据透视表的字段列表。

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


获取基于已保存文件的 CountryCode 的工作簿版本的用户界面语言。

参见 [CountryCode](../../com.aspose.cells/countrycode)。

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


获取此工作簿使用的区域设置。

**Remarks**

如果既未设置 Locale，也未设置 [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--)，则返回 null。

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


获取最大列索引（从零开始）。

**Remarks**

如果文件格式为 Excel97-2003，则返回 255；

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


获取最大行索引（从零开始）。

**Remarks**

如果文件格式为 Excel97-2003，则返回 65535；

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


获取共享公式的最大行号。

**Remarks**

如果数字过大，自动筛选在 MS Excel 2013 中运行会非常慢。

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


获取每个字段唯一项的限制。

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


获取内存使用选项。新选项将作为新建工作表的默认选项，但对已有工作表不生效。

参见 [MemorySetting](../../com.aspose.cells/memorysetting)。

**Remarks**

有关内存模式的更多详细信息，请参见 [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--)。

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


获取数值格式化/解析时的十进制分隔符。默认是当前地区的十进制分隔符。

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


获取数值中小数点左侧数字分组的分隔字符。默认是当前地区的分组分隔符。

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


获取默认打印纸张尺寸。

参见 [PaperSizeType](../../com.aspose.cells/papersizetype)。

**Remarks**

如果没有纸张大小设置，MS Excel 将使用默认打印机的设置。

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


表示工作簿文件的加密密码。

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


指示此工作簿中所有图表的数据点属性和数据标签是否遵循其引用。

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


获取工作簿的保护类型。

参见 [ProtectionType](../../com.aspose.cells/protectiontype)。

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


指示在将以单引号开头的字符串值输入单元格时，是否设置 [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) 属性。

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


获取工作簿的区域设置。

参见 [CountryCode](../../com.aspose.cells/countrycode)。

**Remarks**

1. Aspose.Cells 组件在从模板文件加载工作簿时使用的区域设置：i). 对于 XLS 文件，文件中定义了区域设置字段，MS Excel 在保存 XLS 文件时会将区域设置信息保存到文件中。因此，我们使用模板文件中保存的区域作为工作簿的区域。如果不想使用 XLS 文件中保存的区域，请在加载模板文件后将其重置为期望的值（例如 CountryCode.Default）。同时，在保存 XLS 文件时，我们也会将通过此方法指定的用户值保存到文件中。ii). 对于其他文件格式，如 XLSX、XLSB 等，文件格式规范中未定义区域设置字段。因此，我们使用应用程序环境的区域设置作为工作簿的区域。而通过此方法指定的用户值在生成这些文件格式时无法保留。2. 在 MS Excel 中的查看效果：此处应用的区域设置仅在使用 Aspose.Cells 组件运行时生效，查看生成的文件时不会生效。即使是已保存了指定区域设置信息的生成的 XLS 文件，在使用 MS Excel 查看/编辑时，MS Excel 执行格式化时使用的区域始终是运行 MS Excel 的环境的默认区域设置，而不是文件中保存的区域。这是 MS Excel 的行为，代码无法改变。

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


如果可以从指定的工作簿中删除个人信息，则为 True。

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


指示应用程序上次是否以安全模式或修复模式打开工作簿。

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


获取外部资源的流提供程序，例如加载类型为 "LinkToFile" 的图片的图像数据。

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShapeDisplayType() {#getShapeDisplayType--}
```
public int getShapeDisplayType()
```


获取应用程序在此工作簿中显示形状的方式

请参阅 [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype)。

**Returns:**
int
### getShared() {#getShared--}
```
public boolean getShared()
```


获取指示工作簿是否共享的值。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


工作表选项卡栏的宽度（以窗口宽度的千分之一为单位）。

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


获取工作簿选项卡是否显示的值。

**Remarks**

默认值为 true。

**Example**

以下代码隐藏工作表选项卡和选项卡滚动按钮。

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


获取有效数字的位数。默认值为 [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--)。

**Remarks**

现在只能是 15 或 17。注意：此成员已过时。请改用 [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--)。此属性将在自 2025 年 6 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


获取此工作簿中输出数值的有效数字类型。默认值为 [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--)。

参见 [SignificantDigitsType](../../com.aspose.cells/significantdigitstype)。

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


获取智能标签的选项。

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


获取外部资源的流提供程序。

**Remarks**

注意：此成员已过时。请改用 ResourceProvider 属性。此属性将在自 2022 年 6 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


获取默认主题字体名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype)。字体的方案类型。 |

**Returns:**
java.lang.String -
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


指示是否更新相邻单元格的边框。

**Remarks**

默认值为 false。例如：单元格 A1 的底部边框已更新，单元格 A2 的顶部边框也应相应更改。

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


获取工作簿打开时如何更新外部链接。

请参阅 [UpdateLinksType](../../com.aspose.cells/updatelinkstype)。

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


获取警告回调。

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


窗口的高度，单位为点。

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


窗口的高度，单位为厘米。

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


窗口的高度，单位为英寸。

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


从客户端区域左边缘到窗口左边缘的距离，单位为点。

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


从客户端区域左边缘到窗口左边缘的距离。单位为厘米。

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


从客户端区域左边缘到窗口左边缘的距离。单位为英寸。

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


从客户端区域顶部到窗口顶部的距离，单位为点。

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


从客户端区域顶部到窗口顶部的距离，单位为厘米。

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


从客户端区域顶部到窗口顶部的距离，单位为英寸。

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


窗口的宽度，单位为点。

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


窗口的宽度，单位为厘米。

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


窗口的宽度，单位为英寸。

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


指示是否兼容 WPS。

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


提供对工作簿写保护选项的访问。

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


指示在工作簿的结构和窗口被锁定时是否使用默认密码对工作簿进行加密。

**Remarks**

默认值现在为 false。它与 MS Excel 2013 相同。

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


获取指示是否需要密码才能打开此工作簿的值。

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


获取指示生成的电子表格是否包含水平滚动条的值。

**Remarks**

默认值为 true。

**Example**

以下代码使工作表的水平滚动条不可见。

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


指示此工作簿是否隐藏。

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


表示生成的电子表格是否以最小化方式打开。

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


获取指示工作簿的结构或窗口是否受保护的值。

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


获取指示生成的电子表格是否包含垂直滚动条的值。

**Remarks**

默认值为 true。

**Example**

以下代码使工作表的垂直滚动条不可见。

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


设置文件的作者。

**Remarks**

它未设置，请先检查 [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--)，然后检查 Environment 的用户。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


指定一个布尔值，指示应用程序是否自动压缩工作簿中的图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


指示文件是否标记为自动恢复。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


指定应用程序的增量公开发布版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


指示在保存工作簿时是否检查与早期版本的兼容性。

**Remarks**

默认值为 true。仅适用于 Excel97-2003 的 xls 或 xlt 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


指示在设置 Style.Custom 时是否检查自定义数字格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您的输入字符串作为单元格的值，以便稍后能够将完整的字符串值输出为 CSV 等其他文件格式。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式，否则生成的 Excel 文件可能会出现意外错误。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


指定输出文档的 OOXML 版本。默认值为 Ecma376\_2006。

参见 [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance)。

**Remarks**

仅适用于 .xlsx 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


指示应用程序在崩溃后是否最后一次保存了工作簿文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


指示应用程序是否最后一次打开工作簿以进行数据恢复。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


设置表示工作簿是否使用 1904 日期系统的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


指示在工作簿的结构和窗口被锁定时是否使用默认密码对工作簿进行加密。

**Remarks**

默认值现在为 false。它与 MS Excel 2013 相同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


设置图像的默认分辨率。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


指示是否丢弃编辑的图像数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


指示是否以及如何在工作簿中显示对象。

参见 [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


启用宏；

**Remarks**

目前仅在将工作表复制到同一工作簿的其他工作表时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


设置第一个可见的工作表标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


设置全球化设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


设置指示生成的电子表格是否包含水平滚动条的值。

**Remarks**

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


指示此工作簿是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


设置是否隐藏透视表的字段列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


根据保存文件的 CountryCode 设置工作簿版本的用户界面语言。

参见 [CountryCode](../../com.aspose.cells/countrycode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


设置此工作簿使用的区域设置。

**Remarks**

如果既未设置 Locale，也未设置 [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--)，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


设置共享公式的最大行号。

**Remarks**

如果数字过大，自动筛选在 MS Excel 2013 中运行会非常慢。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


设置每个字段的唯一项限制。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


设置内存使用选项。新选项将作为新建工作表的默认选项，但对已有工作表不生效。

参见 [MemorySetting](../../com.aspose.cells/memorysetting)。

**Remarks**

有关内存模式的更多详细信息，请参见 [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


表示生成的电子表格是否以最小化方式打开。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


设置数值格式化/解析的十进制分隔符。默认值为当前地区的十进制分隔符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


设置十进制左侧数字分组的分隔字符。默认值为当前地区的分组分隔符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


设置整个工作簿的打印方向类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype)。页面方向类型 |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


设置默认打印纸张尺寸。

参见 [PaperSizeType](../../com.aspose.cells/papersizetype)。

**Remarks**

如果没有纸张大小设置，MS Excel 将使用默认打印机的设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


表示工作簿文件的加密密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


指示此工作簿中所有图表的数据点属性和数据标签是否遵循其引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


指示在将以单引号开头的字符串值输入单元格时，是否设置 [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) 属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


设置工作簿的区域设置。

参见 [CountryCode](../../com.aspose.cells/countrycode)。

**Remarks**

1. Aspose.Cells 组件在从模板文件加载工作簿时使用的区域设置：i). 对于 XLS 文件，文件中定义了区域设置字段，MS Excel 在保存 XLS 文件时会将区域设置信息保存到文件中。因此，我们使用模板文件中保存的区域作为工作簿的区域。如果不想使用 XLS 文件中保存的区域，请在加载模板文件后将其重置为期望的值（例如 CountryCode.Default）。同时，在保存 XLS 文件时，我们也会将通过此方法指定的用户值保存到文件中。ii). 对于其他文件格式，如 XLSX、XLSB 等，文件格式规范中未定义区域设置字段。因此，我们使用应用程序环境的区域设置作为工作簿的区域。而通过此方法指定的用户值在生成这些文件格式时无法保留。2. 在 MS Excel 中的查看效果：此处应用的区域设置仅在使用 Aspose.Cells 组件运行时生效，查看生成的文件时不会生效。即使是已保存了指定区域设置信息的生成的 XLS 文件，在使用 MS Excel 查看/编辑时，MS Excel 执行格式化时使用的区域始终是运行 MS Excel 的环境的默认区域设置，而不是文件中保存的区域。这是 MS Excel 的行为，代码无法改变。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


如果可以从指定的工作簿中删除个人信息，则为 True。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


指示应用程序上次是否以安全模式或修复模式打开工作簿。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


设置外部资源的流提供程序，例如加载类型为 "LinkToFile" 的图片数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShapeDisplayType(int value) {#setShapeDisplayType-int-}
```
public void setShapeDisplayType(int value)
```


设置应用程序在此工作簿中显示形状的方式

请参阅 [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


设置一个值，指示工作簿是否已共享。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


工作表选项卡栏的宽度（以窗口宽度的千分之一为单位）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


设置是否显示工作簿标签页的值。

**Remarks**

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


设置有效数字的位数。默认值为 [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--)。

**Remarks**

现在只能是 15 或 17。注意：此成员已过时。请改用 [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--)。此属性将在自 2025 年 6 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


设置此工作簿中输出数值的有效数字类型。默认值为 [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--)。

参见 [SignificantDigitsType](../../com.aspose.cells/significantdigitstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


设置外部资源的流提供程序。

**Remarks**

注意：此成员已过时。请改用 ResourceProvider 属性。此属性将在自 2022 年 6 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


指示是否更新相邻单元格的边框。

**Remarks**

默认值为 false。例如：单元格 A1 的底部边框已更新，单元格 A2 的顶部边框也应相应更改。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


设置工作簿打开时如何更新外部链接。

请参阅 [UpdateLinksType](../../com.aspose.cells/updatelinkstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


设置一个值，指示生成的电子表格是否包含垂直滚动条。

**Remarks**

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


设置警告回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


窗口的高度，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


窗口的高度，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


窗口的高度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


从客户端区域左边缘到窗口左边缘的距离，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


从客户端区域左边缘到窗口左边缘的距离。单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


从客户端区域左边缘到窗口左边缘的距离。单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


从客户端区域顶部到窗口顶部的距离，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


从客户端区域顶部到窗口顶部的距离，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


从客户端区域顶部到窗口顶部的距离，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


窗口的宽度，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


窗口的宽度，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


窗口的宽度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


指示是否兼容 WPS。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

