---
title: "Cells 类"
linktitle: "Cells"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Cells 类。封装了在 Go 中表示单元格的对象。"
type: docs
weight: 200
url: /zh/go-cpp/cells/
---

## Cells class

封装与单元格相关的对象集合，例如 <see cref=\"Cell\"/>、<see cref=\"Row\"/> 等。

```go

type Cells struct  {
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
| [GetOdsCellFields](./getodscellfields/) | 获取 ods 的字段列表。 |
| [Dispose](./dispose/) | 执行应用程序定义的任务，涉及释放、释放或重置非托管资源。 |
| [GetCount](./getcount/) | 获取已实例化 Cell 对象的总数。 |
| [GetCountLarge](./getcountlarge/) | 获取已实例化 Cell 对象的总数。 |
| [GetEnumerator](./getenumerator/) | 获取 cells 枚举器。 |
| [GetRows](./getrows/) | 获取 Row 对象的集合，该集合表示此工作表中的各个行。 |
| [GetMergedAreas](./getmergedareas/) | 获取所有合并的单元格。 |
| [CheckCell](./checkcell/) | 获取在指定单元格行索引和列索引处的 Cell 元素，若不存在则返回 null。 |
| [CheckRow](./checkrow/) | 获取在指定单元格行索引处的 Row 元素，若不存在则返回 null。 |
| [CheckColumn](./checkcolumn/) | 获取在指定列索引处的 Column 元素，若不存在则返回 null。 |
| [IsRowHidden](./isrowhidden/) | 检查给定索引处的行是否隐藏。 |
| [IsColumnHidden](./iscolumnhidden/) | 检查给定索引处的列是否隐藏。 |
| [AddRange](./addrange/) | 向单元格添加范围对象引用 |
| [CreateRange_String_String](./createrange_string_string/) | 从一组单元格创建 Range 对象。 |
| [CreateRange_Int_Int_Int_Int](./createrange_int_int_int_int/) | 从一组单元格创建 Range 对象。 |
| [CreateRange_String](./createrange_string/) | 从范围地址创建 Range 对象。 |
| [CreateRange_Int_Int_Bool](./createrange_int_int_bool/) | 从行或列的单元格创建 Range 对象。 |
| [Get_Int_Int](./get_int_int/) | 获取指定单元格行索引和列索引处的 Cell 元素。 |
| [Get_String](./get_string/) | 获取指定单元格名称处的 Cell 元素。 |
| [GetMultiThreadReading](./getmultithreadreading/) | 获取或设置单元格数据模型是否应支持多线程读取。此属性的默认值为 false。 |
| [SetMultiThreadReading](./setmultithreadreading/) | 获取或设置单元格数据模型是否应支持多线程读取。此属性的默认值为 false。 |
| [GetMemorySetting](./getmemorysetting/) | 获取或设置此单元格的内存使用选项。 |
| [SetMemorySetting](./setmemorysetting/) | 获取或设置此单元格的内存使用选项。 |
| [Clear](./clear/) | 清除工作表的所有数据。 |
| [GetStyle](./getstyle/) | 获取和设置工作表的默认样式。 |
| [SetStyle](./setstyle/) | 获取和设置工作表的默认样式。 |
|[IsDefaultColumnHidden](./isdefaultcolumnhidden/) |  | 
|[SetIsDefaultColumnHidden](./setisdefaultcolumnhidden/) |  | 
| [GetStandardWidthInch](./getstandardwidthinch/) | 获取或设置工作表中列的默认宽度（单位为英寸）。 |
| [SetStandardWidthInch](./setstandardwidthinch/) | 获取或设置工作表中列的默认宽度（单位为英寸）。 |
| [GetStandardWidthPixels](./getstandardwidthpixels/) | 获取或设置工作表中列的默认宽度（单位为像素）。 |
| [SetStandardWidthPixels](./setstandardwidthpixels/) | 获取或设置工作表中列的默认宽度（单位为像素）。 |
| [GetStandardWidth](./getstandardwidth/) | 获取或设置工作表中列的默认宽度（单位为字符）。 |
| [SetStandardWidth](./setstandardwidth/) | 获取或设置工作表中列的默认宽度（单位为字符）。 |
| [GetStandardHeight](./getstandardheight/) | 获取或设置此工作表中行的默认高度（单位为点）。 |
| [SetStandardHeight](./setstandardheight/) | 获取或设置此工作表中行的默认高度（单位为点）。 |
| [GetStandardHeightPixels](./getstandardheightpixels/) | 获取或设置此工作表中行的默认高度（单位为像素）。 |
| [SetStandardHeightPixels](./setstandardheightpixels/) | 获取或设置此工作表中行的默认高度（单位为像素）。 |
| [GetStandardHeightInch](./getstandardheightinch/) | 获取或设置此工作表中行的默认高度（单位为英寸）。 |
| [SetStandardHeightInch](./setstandardheightinch/) | 获取或设置此工作表中行的默认高度（单位为英寸）。 |
| [ImportFormulaArray](./importformulaarray/) | 将公式数组导入工作表。 |
| [TextToColumns](./texttocolumns/) | 将指定列的内容拆分为多个列。 |
| [ImportCSV_String_String_Bool_Int_Int](./importcsv_string_string_bool_int_int/) | 将 CSV 文件导入单元格。 |
| [ImportCSV_Stream_String_Bool_Int_Int](./importcsv_stream_string_bool_int_int/) | 将 CSV 文件导入单元格。 |
| [ImportCSV_String_TxtLoadOptions_Int_Int](./importcsv_string_txtloadoptions_int_int/) | 将 CSV 文件导入单元格。 |
| [ImportCSV_Stream_TxtLoadOptions_Int_Int](./importcsv_stream_txtloadoptions_int_int/) | 将 CSV 文件导入单元格。 |
| [GetPreserveString](./getpreservestring/) | 获取或设置一个值，指示是否将所有工作表值保留为字符串。默认值为 false。 |
| [SetPreserveString](./setpreservestring/) | 获取或设置一个值，指示是否将所有工作表值保留为字符串。默认值为 false。 |
| [Merge_Int_Int_Int_Int](./merge_int_int_int_int/) | 将指定范围的单元格合并为一个单元格。 |
| [Merge_Int_Int_Int_Int_Bool](./merge_int_int_int_int_bool/) | 将指定范围的单元格合并为一个单元格。 |
| [Merge_Int_Int_Int_Int_Bool_Bool](./merge_int_int_int_int_bool_bool/) | 将指定范围的单元格合并为一个单元格。 |
| [UnMerge](./unmerge/) | 取消合并指定范围的已合并单元格。 |
| [ClearMergedCells](./clearmergedcells/) | 清除所有合并的范围。 |
| [HideRow](./hiderow/) | 隐藏一行。 |
| [UnhideRow](./unhiderow/) | 取消隐藏一行。 |
| [HideRows](./hiderows/) | 隐藏多行。 |
| [UnhideRows](./unhiderows/) | 取消隐藏已隐藏的行。 |
| [SetRowHeightPixel](./setrowheightpixel/) | 以像素为单位设置行高。 |
| [SetRowHeightInch](./setrowheightinch/) | 以英寸为单位设置行高。 |
| [SetRowHeight](./setrowheight/) | 设置指定行的高度。 |
| [GetRowHeight_Int_Bool_CellsUnitType](./getrowheight_int_bool_cellsunittype/) | 获取行的高度。 |
| [GetColumnWidth_Int_Bool_CellsUnitType](./getcolumnwidth_int_bool_cellsunittype/) | 获取列宽。 |
| [HideColumn](./hidecolumn/) | 隐藏列。 |
| [UnhideColumn](./unhidecolumn/) | 取消隐藏列 |
| [HideColumns](./hidecolumns/) | 隐藏多列。 |
| [UnhideColumns](./unhidecolumns/) | 取消隐藏多列。 |
| [GetRowHeight_Int](./getrowheight_int/) | 以点为单位获取指定行的高度。 |
| [GetViewRowHeight](./getviewrowheight/) | 获取指定行的高度。 |
| [GetRowHeightInch](./getrowheightinch/) | 以英寸为单位获取指定行的高度。 |
| [GetViewRowHeightInch](./getviewrowheightinch/) | 以英寸为单位获取指定行的高度。 |
| [GetRowHeightPixel](./getrowheightpixel/) | 以像素为单位获取指定行的高度。 |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | 在普通视图中以像素为单位设置列宽。 |
| [SetColumnWidthInch](./setcolumnwidthinch/) | 在普通视图中以英寸为单位设置列宽。 |
| [SetColumnWidth](./setcolumnwidth/) | 在普通视图中设置指定列的宽度。 |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | 在普通视图中以像素为单位获取指定列的宽度。 |
| [GetColumnWidth_Int](./getcolumnwidth_int/) | 在普通视图中获取指定列的宽度（以字符为单位） |
| [GetViewColumnWidthPixel](./getviewcolumnwidthpixel/) | 获取不同视图类型下的宽度。 |
| [SetViewColumnWidthPixel](./setviewcolumnwidthpixel/) | 在不同视图中设置列宽。 |
| [GetMinRow](./getminrow/) | 包含数据或样式的单元格的最小行索引。 |
| [GetMaxRow](./getmaxrow/) | 包含数据或样式的单元格的最大行索引。 |
| [GetMinColumn](./getmincolumn/) | 已实例化的单元格集合中的最小列索引（不包括为整列定义样式但未实例化任何单元格的列）。 |
| [GetMaxColumn](./getmaxcolumn/) | 集合中已实例化的单元格的最大列索引（不包括为整列定义样式但未实例化任何单元格的列）。 |
| [GetMinDataRow](./getmindatarow/) | 包含数据的单元格的最小行索引。 |
| [GetMaxDataRow](./getmaxdatarow/) | 包含数据的单元格的最大行索引。 |
| [GetMinDataColumn](./getmindatacolumn/) | 包含数据的单元格的最小列索引。 |
| [GetMaxDataColumn](./getmaxdatacolumn/) | 包含数据的单元格的最大列索引。 |
| [GetLastDataRow](./getlastdatarow/) | 获取指定列中包含数据的单元格的最后行索引。 |
| [GetFirstDataRow](./getfirstdatarow/) | 获取指定列中包含数据的单元格的第一行索引。 |
| [IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | 指示行高与默认字体高度匹配 |
| [SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | 指示行高与默认字体高度匹配 |
| [IsDefaultRowHidden](./isdefaultrowhidden/) | 指示该行是否默认隐藏。 |
| [SetIsDefaultRowHidden](./setisdefaultrowhidden/) | 指示该行是否默认隐藏。 |
| [GetColumns](./getcolumns/) | 获取表示此工作表中各列的 Column 对象集合。 |
| [ApplyColumnStyle](./applycolumnstyle/) | 对整列应用格式。 |
| [ApplyRowStyle](./applyrowstyle/) | 对整行应用格式。 |
| [ApplyStyle](./applystyle/) | 对整个工作表应用格式。 |
| [CopyColumns_Cells_Int_Int_Int_PasteOptions](./copycolumns_cells_int_int_int_pasteoptions/) | 复制整列的数据和格式。 |
| [CopyColumn](./copycolumn/) | 复制整列的数据和格式。 |
| [CopyColumns_Cells_Int_Int_Int](./copycolumns_cells_int_int_int/) | 复制多列的数据和格式。 |
| [CopyColumns_Cells_Int_Int_Int_Int](./copycolumns_cells_int_int_int_int/) | 复制所有列的数据和格式。 |
| [CopyRow](./copyrow/) | 复制整行的数据和格式。 |
| [CopyRows_Cells_Int_Int_Int](./copyrows_cells_int_int_int/) | 复制若干整行的数据和格式。 |
| [CopyRows_Cells_Int_Int_Int_CopyOptions](./copyrows_cells_int_int_int_copyoptions/) | 复制若干整行的数据和格式。 |
| [CopyRows_Cells_Int_Int_Int_CopyOptions_PasteOptions](./copyrows_cells_int_int_int_copyoptions_pasteoptions/) | 复制若干整行的数据和格式。 |
| [GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | 获取行的轮廓级别（从零开始）。 |
| [GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | 获取列的轮廓级别（从零开始）。 |
| [GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | 获取最大分组列轮廓级别（从零开始）。 |
| [GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | 获取最大分组行轮廓级别（从零开始）。 |
| [ShowGroupDetail](./showgroupdetail/) | 展开分组的行/列。 |
| [HideGroupDetail](./hidegroupdetail/) | 折叠分组的行/列。 |
| [UngroupColumns](./ungroupcolumns/) | 取消列的分组。 |
| [GroupColumns_Int_Int](./groupcolumns_int_int/) | 对列进行分组。 |
| [GroupColumns_Int_Int_Bool](./groupcolumns_int_int_bool/) | 对列进行分组。 |
| [UngroupRows_Int_Int_Bool](./ungrouprows_int_int_bool/) | 取消对行的分组。 |
| [UngroupRows_Int_Int](./ungrouprows_int_int/) | 取消对行的分组。 |
| [GroupRows_Int_Int_Bool](./grouprows_int_int_bool/) | 对行进行分组。 |
| [GroupRows_Int_Int](./grouprows_int_int/) | 对行进行分组。 |
| [DeleteColumn_Int_Bool](./deletecolumn_int_bool/) | 删除一列。 |
| [DeleteColumn_Int](./deletecolumn_int/) | 删除一列。 |
| [DeleteColumns_Int_Int_Bool](./deletecolumns_int_int_bool/) | 删除多列。 |
| [DeleteColumns_Int_Int_DeleteOptions](./deletecolumns_int_int_deleteoptions/) | 删除多列。 |
| [IsDeletingRangeEnabled](./isdeletingrangeenabled/) | 检查范围是否可以删除。 |
| [DeleteRow_Int](./deleterow_int/) | 删除一行。 |
| [DeleteRow_Int_Bool](./deleterow_int_bool/) | 删除一行。 |
| [DeleteRows_Int_Int](./deleterows_int_int/) | 删除多行。 |
| [DeleteRows_Int_Int_Bool](./deleterows_int_int_bool/) | 在工作表中删除多行。 |
| [DeleteRows_Int_Int_DeleteOptions](./deleterows_int_int_deleteoptions/) | 在工作表中删除多行。 |
| [DeleteBlankColumns](./deleteblankcolumns/) | 删除所有不包含任何数据的空列。 |
| [DeleteBlankColumns_DeleteOptions](./deleteblankcolumns_deleteoptions/) | 删除所有不包含任何数据的空列。 |
| [IsBlankColumn](./isblankcolumn/) | 检查给定列是否为空（不包含任何数据）。 |
| [DeleteBlankRows](./deleteblankrows/) | 删除所有不包含任何数据或其他对象的空行。 |
| [DeleteBlankRows_DeleteOptions](./deleteblankrows_deleteoptions/) | 删除所有不包含任何数据或某些特殊对象（如可见批注、数据透视表）的空行。 |
| [InsertColumns_Int_Int](./insertcolumns_int_int/) | 在工作表中插入若干列。 |
| [InsertColumns_Int_Int_Bool](./insertcolumns_int_int_bool/) | 在工作表中插入若干列。 |
| [InsertColumns_Int_Int_InsertOptions](./insertcolumns_int_int_insertoptions/) | 在工作表中插入若干列。 |
| [InsertColumn_Int_Bool](./insertcolumn_int_bool/) | 在工作表中插入新列。 |
| [InsertColumn_Int](./insertcolumn_int/) | 在工作表中插入新列。 |
| [InsertRows_Int_Int_Bool](./insertrows_int_int_bool/) | 在工作表中插入多行。 |
| [InsertRows_Int_Int_InsertOptions](./insertrows_int_int_insertoptions/) | 在工作表中插入多行。 |
| [InsertRows_Int_Int](./insertrows_int_int/) | 在工作表中插入多行。 |
| [InsertRow](./insertrow/) | 在工作表中插入新行。 |
| [GetRanges](./getranges/) | 获取运行时创建的 Range 对象集合。 |
| [ClearRange_CellArea](./clearrange_cellarea/) | 清除范围的内容和格式。 |
| [ClearRange_Int_Int_Int_Int](./clearrange_int_int_int_int/) | 清除范围的内容和格式。 |
| [ClearContents_CellArea](./clearcontents_cellarea/) | 清除范围的内容。 |
| [ClearContents_Int_Int_Int_Int](./clearcontents_int_int_int_int/) | 清除范围的内容。 |
| [ClearFormats_CellArea](./clearformats_cellarea/) | 清除范围的格式。 |
| [ClearFormats_Int_Int_Int_Int](./clearformats_int_int_int_int/) | 清除范围的格式。 |
| [GetLastCell](./getlastcell/) | 获取此工作表中的最后一个单元格。 |
| [LinkToXmlMap](./linktoxmlmap/) | 链接到 XML 映射。 |
| [GetMaxDisplayRange](./getmaxdisplayrange/) | 获取包含数据、合并单元格和形状的最大范围。 |
| [GetFirstCell](./getfirstcell/) | 获取此工作表中的第一个单元格。 |
| [Find_Object_Cell](./find_object_cell/) | 查找包含输入对象的单元格。 |
| [Find_Object_Cell_FindOptions](./find_object_cell_findoptions/) | 查找包含输入对象的单元格。 |
| [EndCellInRow_Int](./endcellinrow_int/) | 获取此行中的最后一个单元格。 |
| [EndCellInColumn_Int](./endcellincolumn_int/) | 获取此列中的最后一个单元格。 |
| [EndCellInColumn_Int_Int_Int_Int](./endcellincolumn_int_int_int_int/) | 获取此范围中列索引最大的最后一个单元格。 |
| [EndCellInRow_Int_Int_Int_Int](./endcellinrow_int_int_int_int/) | 获取此范围中行索引最大的最后一个单元格。 |
| [MoveRange](./moverange/) | 移动该范围。 |
| [InsertCutCells](./insertcutcells/) | 插入剪切的范围。 |
| [InsertRange_CellArea_Int_ShiftType_Bool](./insertrange_cellarea_int_shifttype_bool/) | 插入一段单元格，并根据移动选项移动单元格。 |
| [InsertRange_CellArea_ShiftType](./insertrange_cellarea_shifttype/) | 插入一段单元格，并根据移动选项移动单元格。 |
| [InsertRange_CellArea_Int_ShiftType](./insertrange_cellarea_int_shifttype/) | 插入一段单元格，并根据移动选项移动单元格。 |
| [DeleteRange](./deleterange/) | 删除一段单元格，并根据移动选项移动单元格。 |
| [ExportArray](./exportarray/) | 将 Cells 集合中的数据导出为二维数组对象。 |
| [RetrieveSubtotalSetting](./retrievesubtotalsetting/) | 检索该范围的汇总设置。 |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array](./subtotal_cellarea_int_consolidationfunction_int32array/) | 为该范围创建汇总。 |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array_Bool_Bool_Bool](./subtotal_cellarea_int_consolidationfunction_int32array_bool_bool_bool/) | 为该范围创建汇总。 |
| [RemoveFormulas](./removeformulas/) | 删除所有公式并替换为公式的计算值。 |
| [RemoveDuplicates](./removeduplicates/) | 删除工作表中的重复行。 |
| [RemoveDuplicates_Int_Int_Int_Int](./removeduplicates_int_int_int_int/) | 删除范围内的重复值。 |
| [RemoveDuplicates_Int_Int_Int_Int_Bool_int32Array](./removeduplicates_int_int_int_int_bool_int32array/) | 删除范围内的重复数据。 |
| [ConvertStringToNumericValue](./convertstringtonumericvalue/) | 如果可能，将工作表中的所有字符串数据转换为数值。 |
| [GetDependents](./getdependents/) | 获取所有引用特定单元格的单元格。 |
| [GetDependentsInCalculation](./getdependentsincalculation/) | 获取所有计算结果依赖于特定单元格的单元格。 |
| [GetCellsWithPlaceInCellPicture](./getcellswithplaceincellpicture/) | 获取所有包含嵌入图片的单元格。 |
| [GetCellStyle](./getcellstyle/) | 获取给定单元格的样式。 |
| [GetCellDisplayStyle_Int_Int](./getcelldisplaystyle_int_int/) | 获取给定单元格的显示样式。 |
| [GetCellDisplayStyle_Int_Int_BorderType](./getcelldisplaystyle_int_int_bordertype/) | 获取给定单元格的显示样式。 |
