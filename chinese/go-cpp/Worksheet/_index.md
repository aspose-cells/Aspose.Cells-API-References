---
title: "Worksheet 类"
linktitle: "Worksheet"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Worksheet 类。封装了在 Go 中表示工作表的对象。"
type: docs
weight: 200
url: /zh/go-cpp/worksheet/
---

## Worksheet class

封装表示单个工作表的对象。

```go

type Worksheet struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Dispose](./dispose/) | 执行应用程序定义的任务，涉及释放、释放或重置非托管资源。 |
| [GetProtection](./getprotection/) | 表示工作表可用的各种保护选项类型。支持 ExcelXP 及以上版本的高级保护选项。 |
| [GetUniqueId](./getuniqueid/) | 获取和设置唯一 ID， 与 {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F} 相同。 |
| [SetUniqueId](./setuniqueid/) | 获取和设置唯一 ID， 与 {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F} 相同。 |
| [GetPanes](./getpanes/) | 获取窗口窗格。 |
| [GetWorkbook](./getworkbook/) | 获取包含此工作表的工作簿对象。 |
| [GetCells](./getcells/) | 获取 Aspose.Cells.Cells 集合。 |
| [GetQueryTables](./getquerytables/) | 获取工作表中的 QueryTableCollection。 |
| [GetType](./gettype/) | 表示工作表类型。 |
| [SetType](./settype/) | 表示工作表类型。 |
| [GetName](./getname/) | 获取或设置工作表的名称。 |
| [SetName](./setname/) | 获取或设置工作表的名称。 |
| [GetShowFormulas](./getshowformulas/) | 指示是否显示公式或其结果。 |
| [SetShowFormulas](./setshowformulas/) | 指示是否显示公式或其结果。 |
| [GetShowDataTypeIcons](./getshowdatatypeicons/) | 指示是否显示数据类型图标。 |
| [SetShowDataTypeIcons](./setshowdatatypeicons/) | 指示是否显示数据类型图标。 |
| [IsGridlinesVisible](./isgridlinesvisible/) | 获取或设置指示网格线是否可见的值。默认值为 true。 |
| [SetIsGridlinesVisible](./setisgridlinesvisible/) | 获取或设置指示网格线是否可见的值。默认值为 true。 |
| [IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | 获取或设置指示工作表是否显示行和列标题的值。默认值为 true。 |
| [SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | 获取或设置指示工作表是否显示行和列标题的值。默认值为 true。 |
| [GetPaneState](./getpanestate/) | 指示窗格是否具有水平或垂直拆分，以及这些拆分是否已冻结。 |
| [GetDisplayZeros](./getdisplayzeros/) | 如果显示零值，则为 true。 |
| [SetDisplayZeros](./setdisplayzeros/) | 如果显示零值，则为 true。 |
| [GetDisplayRightToLeft](./getdisplayrighttoleft/) | 指示指定的工作表是否从右向左显示，而不是从左向右显示。默认值为 false。 |
| [SetDisplayRightToLeft](./setdisplayrighttoleft/) | 指示指定的工作表是否从右向左显示，而不是从左向右显示。默认值为 false。 |
| [IsOutlineShown](./isoutlineshown/) | 指示是否显示大纲。 |
| [SetIsOutlineShown](./setisoutlineshown/) | 指示是否显示大纲。 |
| [IsSelected](./isselected/) | 指示打开工作簿时是否选中此工作表。 |
| [SetIsSelected](./setisselected/) | 指示打开工作簿时是否选中此工作表。 |
| [FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | 在工作表的指定单元格处冻结窗格。 |
| [GetFreezedPanes](./getfreezedpanes/) | 获取冻结的窗格。 |
| [Split](./split/) | 拆分窗口。 |
| [FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | 在工作表的指定单元格处冻结窗格。 |
| [UnFreezePanes](./unfreezepanes/) | 取消工作表中的窗格冻结。 |
| [RemoveSplit](./removesplit/) | 移除拆分窗口。 |
| [GetPivotTables](./getpivottables/) | 获取此工作表中的所有数据透视表。 |
| [GetListObjects](./getlistobjects/) | 获取此工作表中的所有 ListObjects。 |
| [GetTabId](./gettabid/) | 指定工作表的内部标识符。 |
| [SetTabId](./settabid/) | 指定工作表的内部标识符。 |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | 获取 HorizontalPageBreakCollection 集合。 |
| [GetVerticalPageBreaks](./getverticalpagebreaks/) | 获取 VerticalPageBreakCollection 集合。 |
| [AddPageBreaks](./addpagebreaks/) | 添加分页符。 |
| [GetHyperlinks](./gethyperlinks/) | 获取 HyperlinkCollection 集合。 |
| [Copy_Worksheet](./copy_worksheet/) | 从另一个工作表复制内容和格式。 |
| [Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | 从另一个工作表复制内容和格式。 |
| [AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | 自动调整列宽。 |
| [AutoFitColumns](./autofitcolumns/) | 自动调整此工作表中所有列的宽度。 |
| [AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | 自动调整此工作表中所有列的宽度。 |
| [AutoFitColumn_Int](./autofitcolumn_int/) | 自动调整列宽。 |
| [AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | 自动调整列宽。 |
| [AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | 自动调整列宽。 |
| [AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | 自动调整列宽。 |
| [AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | 自动调整列宽。 |
| [AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | 自动调整行高。 |
| [AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | 自动调整行高。 |
| [AutoFitRows](./autofitrows/) | 自动调整此工作表中所有行的高度。 |
| [AutoFitRows_Bool](./autofitrows_bool/) | 自动调整此工作表中所有行的高度。 |
| [AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | 自动调整此工作表中所有行的高度。 |
| [AutoFitRows_Int_Int](./autofitrows_int_int/) | 在范围内自动调整行高。 |
| [AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | 在范围内自动调整行高。 |
| [AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | 在矩形范围内自动调整行高。 |
| [AutoFitRow_Int](./autofitrow_int/) | 自动调整行高。 |
| [GetPageSetup](./getpagesetup/) | 表示此工作表的页面设置描述。 |
| [GetAutoFilter](./getautofilter/) | 表示指定工作表的自动筛选。 |
| [Filter](./filter/) | 筛选该范围。 |
| [GetAdvancedFilter](./getadvancedfilter/) | 获取高级筛选的设置。 |
| [Advanced_Filter](./advanced_filter/) | 使用复杂条件筛选数据。 |
| [RemoveAutoFilter](./removeautofilter/) | 移除工作表的自动筛选。 |
| [GetHasAutofilter](./gethasautofilter/) | 指示此工作表是否具有自动筛选。 |
| [GetTransitionEvaluation](./gettransitionevaluation/) | 指示是否启用了过渡公式评估（Lotus 兼容性）选项。 |
| [SetTransitionEvaluation](./settransitionevaluation/) | 指示是否启用了过渡公式评估（Lotus 兼容性）选项。 |
| [GetTransitionEntry](./gettransitionentry/) | 指示是否启用了过渡公式输入（Lotus 兼容性）选项。 |
| [SetTransitionEntry](./settransitionentry/) | 指示是否启用了过渡公式输入（Lotus 兼容性）选项。 |
| [GetVisibilityType](./getvisibilitytype/) | 指示此工作表的可见状态。 |
| [SetVisibilityType](./setvisibilitytype/) | 指示此工作表的可见状态。 |
| [SetVisible](./setvisible/) | 设置可见选项。 |
| [IsVisible](./isvisible/) | 表示工作表是否可见。 |
| [SetIsVisible](./setisvisible/) | 表示工作表是否可见。 |
| [SelectRange](./selectrange/) | 选择一个范围。 |
| [RemoveAllDrawingObjects](./removealldrawingobjects/) | 删除此工作表中的所有绘图对象。 |
| [ClearComments](./clearcomments/) | 清除设计器电子表格中的所有批注。 |
| [GetSparklineGroups](./getsparklinegroups/) | 获取工作表中的微型图组。 |
| [GetCharts](./getcharts/) | 获取图表集合 |
| [GetComments](./getcomments/) | 获取批注集合。 |
| [GetPictures](./getpictures/) | 获取图片集合。 |
| [GetAllPictures](./getallpictures/) | 获取所有图片，包括嵌入单元格和覆盖单元格的图像。 |
| [GetTextBoxes](./gettextboxes/) | 获取文本框集合。 |
| [GetCheckBoxes](./getcheckboxes/) | 获取复选框集合。 |
| [GetOleObjects](./getoleobjects/) | 表示工作表中 OleObject 的集合。 |
| [GetShapes](./getshapes/) | 返回此工作表中的所有绘图形状。 |
| [GetSlicers](./getslicers/) | 获取工作表中的切片器集合 |
| [GetTimelines](./gettimelines/) | 获取工作表中的时间轴集合 |
| [Protect_ProtectionType](./protect_protectiontype/) | 保护工作表。 |
| [Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | 保护工作表。 |
| [Unprotect](./unprotect/) | 取消保护工作表。 |
| [Unprotect_String](./unprotect_string/) | 取消保护工作表。 |
| [GetIndex](./getindex/) | 获取工作表集合中工作表的索引。 |
| [MoveTo](./moveto/) | 将工作表移动到电子表格中的其他位置。 |
| [IsProtected](./isprotected/) | 指示工作表是否受保护。 |
| [GetValidations](./getvalidations/) | 获取工作表中的数据验证设置集合。 |
| [GetAllowEditRanges](./getalloweditranges/) | 获取工作表中的允许编辑范围集合。 |
| [GetErrorCheckOptions](./geterrorcheckoptions/) | 获取对特定范围应用的错误检查设置。 |
| [GetOutline](./getoutline/) | 获取此工作表的轮廓。 |
| [GetFirstVisibleRow](./getfirstvisiblerow/) | 表示第一可见行索引。 |
| [SetFirstVisibleRow](./setfirstvisiblerow/) | 表示第一可见行索引。 |
| [GetFirstVisibleColumn](./getfirstvisiblecolumn/) | 表示第一可见列索引。 |
| [SetFirstVisibleColumn](./setfirstvisiblecolumn/) | 表示第一可见列索引。 |
| [Replace](./replace/) | 将所有单元格的文本替换为新字符串。 |
| [GetZoom](./getzoom/) | 表示以百分比计的缩放因子。它应在 10 到 400 之间。 |
| [SetZoom](./setzoom/) | 表示以百分比计的缩放因子。它应在 10 到 400 之间。 |
| [GetViewType](./getviewtype/) | 获取和设置视图类型。 |
| [SetViewType](./setviewtype/) | 获取和设置视图类型。 |
| [IsPageBreakPreview](./ispagebreakpreview/) | 指示指定的工作表是以普通视图还是分页预览方式显示。 |
| [SetIsPageBreakPreview](./setispagebreakpreview/) | 指示指定的工作表是以普通视图还是分页预览方式显示。 |
| [IsRulerVisible](./isrulervisible/) | 指示标尺是否可见。此属性仅在分页预览时适用。 |
| [SetIsRulerVisible](./setisrulervisible/) | 指示标尺是否可见。此属性仅在分页预览时适用。 |
| [GetSelectedAreas](./getselectedareas/) | 获取设计器电子表格中选定的单元格范围。 |
| [GetTabColor](./gettabcolor/) | 表示工作表标签颜色。 |
| [SetTabColor](./settabcolor/) | 表示工作表标签颜色。 |
| [GetGridlineColor](./getgridlinecolor/) | 获取和设置网格线的颜色 |
| [SetGridlineColor](./setgridlinecolor/) | 获取和设置网格线的颜色 |
| [GetCodeName](./getcodename/) | 获取工作表代码名称。 |
| [SetCodeName](./setcodename/) | 获取工作表代码名称。 |
| [GetBackgroundImage](./getbackgroundimage/) | 获取和设置工作表背景图像。 |
| [SetBackgroundImage](./setbackgroundimage/) | 获取和设置工作表背景图像。 |
| [GetConditionalFormattings](./getconditionalformattings/) | 获取工作表中的条件格式。 |
| [GetActiveCell](./getactivecell/) | 获取或设置工作表中的活动单元格。 |
| [SetActiveCell](./setactivecell/) | 获取或设置工作表中的活动单元格。 |
| [GetCustomProperties](./getcustomproperties/) | 获取表示与工作表关联的标识信息的对象。 |
| [GetPrintingPageBreaks](./getprintingpagebreaks/) | 获取自动分页符。 |
| [GetSmartTagSetting](./getsmarttagsetting/) | 获取工作表的所有 SmartTagCollection 对象。 |
| [ToString](./tostring/) | 返回表示当前 Worksheet 对象的字符串。 |
| [GetScenarios](./getscenarios/) | 获取 Scenario 集合。 |
| [StartAccessCache](./startaccesscache/) | 启动使用缓存访问此工作表数据的会话。 |
| [CloseAccessCache](./closeaccesscache/) | 关闭使用缓存访问此工作表数据的会话。 |
| [ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | 转换公式引用样式。 |
| [CalculateFormula_String](./calculateformula_string/) | 计算公式。 |
| [CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | 直接计算公式表达式。 |
| [CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | 直接计算公式表达式。 |
| [CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | 将公式计算为数组公式。 |
| [CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | 将公式计算为数组公式。 |
| [CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | 将公式计算为数组公式。 |
| [CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | 计算此工作表中的所有公式。 |
| [GetAreasOfXmlMapQuery](./getareasofxmlmapquery/) | 查询映射/链接到 XML 映射特定路径的单元格区域。 |
| [GetCellWatches](./getcellwatches/) | 获取在此工作表中被 'watch window' 监视的单元格集合。 |
| [RefreshPivotTables](./refreshpivottables/) | 刷新此工作表中的所有数据透视表。 |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | 刷新此工作表中的所有数据透视表。 |
