---
title: "ExternalConnection.ConnectionDescription"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحدد وصف المستخدم لهذا الاتصال"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/connectiondescription/
---
## ExternalConnection.ConnectionDescription property

يحدد الوصف الذي يدخله المستخدم لهذا الاتصال

```csharp
public string ConnectionDescription { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyConnectionDescriptionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // أضف ورقة عمل ببيانات عينة
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Sales";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1000;
                worksheet.Cells["A3"].Value = "Banana";
                worksheet.Cells["B3"].Value = 2000;

                // أنشئ جدول محوري لإنشاء اتصال خارجي
                int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // الحصول على الاتصال الخارجي من الجدول المحوري.
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // اعرض قيمة ConnectionDescription الأولية
                Console.WriteLine("Initial ConnectionDescription: " + connection.ConnectionDescription);

                // حدد وصفًا جديدًا (نظرًا لأنه قابل للقراءة والكتابة)
                connection.ConnectionDescription = "This connection retrieves sales data from internal sources";
                Console.WriteLine("Updated ConnectionDescription: " + connection.ConnectionDescription);

                // امسح الوصف
                connection.ConnectionDescription = string.Empty;
                Console.WriteLine("Cleared ConnectionDescription: " + connection.ConnectionDescription);

                // احفظ المصنف مع الاتصال المعدل
                workbook.Save("ConnectionDescriptionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


