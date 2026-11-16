---
title: "PivotArea 类"
linktitle: "PivotArea"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotArea 类。封装在 Go 中表示 pivotarea 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotarea/
---

## PivotArea class

表示数据透视表的选定区域。

```go

type PivotArea struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewPivotArea](./newpivotarea/) | 呈现 PivotTable 的选定区域。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetFilters](./getfilters/) | 获取此 PivotArea 的所有过滤器。 |
| [Select](./select/) | 选择带有过滤器的区域。 |
| [SelectField_PivotFieldType_String](./selectfield_pivotfieldtype_string/) | 将区域中的字段选择为一个区域。 |
| [SelectField_PivotFieldType_PivotField](./selectfield_pivotfieldtype_pivotfield/) | 将区域中的字段选择为一个区域。 |
| [GetOnlyData](./getonlydata/) | 指示是否仅选择项目选择的数据显示值（视图的数据区域），且不包括项目标签。 |
| [SetOnlyData](./setonlydata/) | 指示是否仅选择项目选择的数据显示值（视图的数据区域），且不包括项目标签。 |
| [GetOnlyLabel](./getonlylabel/) | 指示是否仅选择项目选择的数据标签。 |
| [SetOnlyLabel](./setonlylabel/) | 指示是否仅选择项目选择的数据标签。 |
| [IsRowGrandIncluded](./isrowgrandincluded/) | 指示是否包含行总计。 |
| [SetIsRowGrandIncluded](./setisrowgrandincluded/) | 指示是否包含行总计。 |
| [IsColumnGrandIncluded](./iscolumngrandincluded/) | 指示是否包含列总计。 |
| [SetIsColumnGrandIncluded](./setiscolumngrandincluded/) | 指示是否包含列总计。 |
| [GetAxisType](./getaxistype/) | 获取并设置此规则适用的 PivotTable 区域。 |
| [SetAxisType](./setaxistype/) | 获取并设置此规则适用的 PivotTable 区域。 |
| [GetRuleType](./getruletype/) | 获取并设置选择规则的类型。 |
| [SetRuleType](./setruletype/) | 获取并设置选择规则的类型。 |
| [IsOutline](./isoutline/) | 指示规则是否引用处于大纲模式的区域。 |
| [SetIsOutline](./setisoutline/) | 指示规则是否引用处于大纲模式的区域。 |
| [GetCellAreas](./getcellareas/) | 获取此数据透视区域的单元格区域。 |
