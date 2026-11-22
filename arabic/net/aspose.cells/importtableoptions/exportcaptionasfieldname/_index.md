---
title: "ImportTableOptions.ExportCaptionAsFieldName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تشير إلى ما إذا كان تصدير العنوان كاسم حقل"
type: docs
url: /ar/net/aspose.cells/importtableoptions/exportcaptionasfieldname/
---
## ImportTableOptions.ExportCaptionAsFieldName property

يشير إلى ما إذا كان يتم تصدير العنوان كاسم الحقل

```csharp
public bool ExportCaptionAsFieldName { get; set; }
```

### ملاحظات

يعمل فقط مع DataTable.

### أمثلة

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
            // إنشاء بيانات نموذجية
            List<Transaction> transactions = new List<Transaction>
            {
                new Transaction { orderId = "w101", paymentType = "card", orderType = "bur" },
                new Transaction { orderId = "w102", paymentType = "cash", orderType = "piz" },
                new Transaction { orderId = "w103", paymentType = "card", orderType = "sal" }
            };

            // إنشاء دفتر عمل واستيراد البيانات مع ExportCaptionAsFieldName
            Workbook workbook = new Workbook();
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.ExportCaptionAsFieldName = true;
            workbook.Worksheets[0].Cells.ImportCustomObjects(transactions, 0, 0, importOptions);

            // تصدير البيانات مرة أخرى للتحقق
            ExportTableOptions exportOptions = new ExportTableOptions();
            List<Transaction> exportedData = workbook.Worksheets[0].Cells.ExportList<Transaction>(0, 0, 5, 10, exportOptions);

            // أخرج التحقق
            Console.WriteLine($"Exported count: {exportedData.Count}");
            Console.WriteLine($"First payment type: {exportedData[0].paymentType}");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


