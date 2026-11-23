---
title: "ImportTableOptions.ExportCaptionAsFieldName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ImportTableOptions 属性。指示是否将标题导出为字段名"
type: docs
url: /zh/net/aspose.cells/importtableoptions/exportcaptionasfieldname/
---
## ImportTableOptions.ExportCaptionAsFieldName property

指示是否将标题导出为字段名

```csharp
public bool ExportCaptionAsFieldName { get; set; }
```

### 备注

仅适用于 DataTable。

### 示例

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyExportCaptionAsFieldNameDemo
    {
        public class Transaction
        {
            public string orderId { get; set; }
            public string paymentType { get; set; }
            public string orderType { get; set; }
        }

        public static void Run()
        {
            // 创建示例数据
            List<Transaction> transactions = new List<Transaction>
            {
                new Transaction { orderId = "w101", paymentType = "card", orderType = "bur" },
                new Transaction { orderId = "w102", paymentType = "cash", orderType = "piz" },
                new Transaction { orderId = "w103", paymentType = "card", orderType = "sal" }
            };

            // 创建工作簿并使用 ExportCaptionAsFieldName 导入数据
            Workbook workbook = new Workbook();
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.ExportCaptionAsFieldName = true;
            workbook.Worksheets[0].Cells.ImportCustomObjects(transactions, 0, 0, importOptions);

            // 导出数据以进行验证
            ExportTableOptions exportOptions = new ExportTableOptions();
            List<Transaction> exportedData = workbook.Worksheets[0].Cells.ExportList<Transaction>(0, 0, 5, 10, exportOptions);

            // 输出验证
            Console.WriteLine($"Exported count: {exportedData.Count}");
            Console.WriteLine($"First payment type: {exportedData[0].paymentType}");
        }
    }
}
```

### 另请参见

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


