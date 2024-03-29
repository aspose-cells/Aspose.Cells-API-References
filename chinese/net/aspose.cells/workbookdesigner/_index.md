---
title: WorkbookDesigner
second_title: Aspose.Cells for .NET API 参考
description: 封装表示设计器电子表格的对象
type: docs
weight: 6490
url: /zh/net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

封装表示设计器电子表格的对象。

```csharp
public class WorkbookDesigner
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [WorkbookDesigner](workbookdesigner#constructor)() | 初始化[`WorkbookDesigner`](../workbookdesigner)类. |
| [WorkbookDesigner](workbookdesigner#constructor_1)(Workbook) | 初始化[`WorkbookDesigner`](../workbookdesigner)类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula) { get; set; } | 表示是否应计算公式。 |
| [CallBack](../../aspose.cells/workbookdesigner/callback) { get; set; } | 获取和设置处理smartmarker的回调接口。 |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline) { get; set; } | 表示是否逐行处理智能标记。 |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal) { get; set; } | 指示是否重复带有小计行的公式。 |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull) { get; set; } | 如果为TRUE，如果值为“”，则插入Null； |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference) { get; set; } | 指示是否将更新其他工作表中的引用。 |
| [Workbook](../../aspose.cells/workbookdesigner/workbook) { get; set; } | 获取并设置[`Workbook`](./workbook)对象. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource)() | 清除所有数据源。 |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers)() | 返回电子表格中智能标记的集合。 |
| [Process](../../aspose.cells/workbookdesigner/process#process)() | 处理智能标记并填充数据源值。 |
| [Process](../../aspose.cells/workbookdesigner/process#process_1)(bool) | 处理智能标记并填充数据源值。 |
| [Process](../../aspose.cells/workbookdesigner/process#process_2)(int, bool) | 处理智能标记并填充数据源值。 |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource#setdatasource)(DataSet) | 设置 DataSet 对象的数据源。 |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource#setdatasource_1)(DataTable) | 设置 DataTable 对象的数据源。 |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource#setdatasource_2)(DataView) | 设置 DataView 对象的数据源。 |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource#setdatasource_3)(OleDbConnection) | 设置 OleDbConnection 对象的数据源。 |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource#setdatasource_4)(SqlConnection) | 设置 SqlConnection 对象的数据源。 |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource#setdatasource_6)(string, DataView) | 设置 DataView 对象的数据源并将其绑定到数据源名称。 |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource#setdatasource_5)(string, ICellsDataTable) | 设置数据源[`ICellsDataTable`](../icellsdatatable)对象. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource#setdatasource_8)(string, object) | 将数据绑定设置为变量。 |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource#setdatasource_7)(string, IDataReader, int) | 设置 IDataReader 对象的数据源。 |

### 例子

```csharp

[C#]

//创建 WorkbookDesigner 对象。
WorkbookDesigner wd = new WorkbookDesigner();
//打开模板文件（包含智能标记）。
wd.Workbook = new Workbook("SmartMarker_Designer.xls");

//从数据源初始化你的数据
//数据集 ds = new DataSet();
//...

//设置数据表为数据源。
//wd.SetDataSource(dt);
//处理智能标记以将数据填充到工作表中。
wd.Process(true);
//保存excel文件。
wd.Workbook.Save("outSmartMarker_Designer.xls");

```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
