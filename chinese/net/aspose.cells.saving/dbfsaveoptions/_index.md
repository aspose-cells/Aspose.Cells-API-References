---
title: "类 DbfSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Saving.DbfSaveOptions 类。表示保存 dbf 文件的选项"
type: docs
url: /zh/net/aspose.cells.saving/dbfsaveoptions/
---
## DbfSaveOptions class

表示保存 dbf 文件的选项

```csharp
public class DbfSaveOptions : SaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [DbfSaveOptions](dbfsaveoptions/)() | 保存 .dbf 文件的选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | 用于临时文件的文件夹，可能用作数据缓存。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当输入的值超过 32K 时，将被截断。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | 在保存文件后使工作簿为空。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | 如果为 true 且目录不存在，则在保存文件之前会自动创建该目录。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [ExportAsString](../../aspose.cells.saving/dbfsaveoptions/exportasstring/) { get; set; } | 指示是否以字符串值导出 |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | 指示在保存文件之前是否合并条件格式和数据验证的区域。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | 指示是否缓存图表的最新数据。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | 获取保存文件的格式。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | 指示在保存文件之前是否对外部已定义的名称进行排序。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | 指示在保存文件之前是否对已定义的名称进行排序。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | 指示是否更新 Smart Art 设置。默认值为 false。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | 指示是否在保存文件之前验证合并单元格。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | 获取或设置警告回调。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassDbfSaveOptionsDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向工作表添加示例数据
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // 创建 DbfSaveOptions 的实例
            DbfSaveOptions saveOptions = new DbfSaveOptions();
            
            // 设置 ExportAsString 属性
            saveOptions.ExportAsString = true;

            // 使用 DBF 保存选项保存工作簿
            workbook.Save("output.dbf", saveOptions);

            Console.WriteLine("Workbook saved as DBF with ExportAsString set to true.");
        }
    }
}
```

### 另请参见

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


