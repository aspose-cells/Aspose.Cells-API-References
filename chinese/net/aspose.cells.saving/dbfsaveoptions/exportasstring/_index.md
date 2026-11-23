---
title: "DbfSaveOptions.ExportAsString"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DbfSaveOptions 属性。指示是否以字符串值导出"
type: docs
url: /zh/net/aspose.cells.saving/dbfsaveoptions/exportasstring/
---
## DbfSaveOptions.ExportAsString property

指示是否以字符串值导出

```csharp
public bool ExportAsString { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加包含混合类型的示例数据
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("TextValue");

            // 创建 DbfSaveOptions 实例
            DbfSaveOptions options = new DbfSaveOptions();

            // 显示当前 ExportAsString 值
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // 将 ExportAsString 设置为 true（所有值将导出为字符串）
            options.ExportAsString = true;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // 在 ExportAsString = true 时保存
            workbook.Save("ExportAsStringTrue.dbf", options);

            // 将 ExportAsString 设置为 false（值将保持其原始类型）
            options.ExportAsString = false;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // 在 ExportAsString = false 时保存
            workbook.Save("ExportAsStringFalse.dbf", options);
        }
    }
}
```

### 另请参见

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


