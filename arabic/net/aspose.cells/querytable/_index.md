---
title: "الفئة QueryTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.QueryTable فئة. يمثل معلومات QueryTable"
type: docs
url: /ar/net/aspose.cells/querytable/
---
## QueryTable class

يمثل معلومات QueryTable.

```csharp
public class QueryTable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | يعيد أو يضبط AdjustColumnWidth للكائن. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | يحصل على معرف الاتصال لجدول الاستعلام. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | يحصل على الاتصال الخارجي المرتبط. |
| [Name](../../aspose.cells/querytable/name/) { get; } | يحصل على اسم querytable. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | يعيد أو يضبط PreserveFormatting للكائن. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | يحصل على نطاق النتيجة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassQueryTableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة لإنشاء جدول استعلام (محاكاة للبيانات الخارجية)
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // تحقق مما إذا كان هناك أي جداول استعلام في ورقة العمل
            if (worksheet.QueryTables.Count > 0)
            {
                // احصل على أول جدول استعلام
                QueryTable qt = worksheet.QueryTables[0];
                
                // عرض خصائص جدول الاستعلام
                Console.WriteLine("Query Table Name: " + qt.Name);
                Console.WriteLine("Connection ID: " + qt.ConnectionId);
                Console.WriteLine("Result Range: " + qt.ResultRange.Address);
                Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);
                Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
                
                // تعديل بعض الخصائص
                qt.PreserveFormatting = true;
                qt.AdjustColumnWidth = false;
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


