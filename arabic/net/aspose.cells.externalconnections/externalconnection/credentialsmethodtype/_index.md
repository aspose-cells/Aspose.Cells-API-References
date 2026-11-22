---
title: "ExternalConnection.CredentialsMethodType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحدد طريقة المصادقة التي يجب استخدامها عند إنشاء أو إعادة إنشاء الاتصال."
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/credentialsmethodtype/
---
## ExternalConnection.CredentialsMethodType property

يحدد طريقة المصادقة التي يجب استخدامها عند إنشاء (أو إعادة إنشاء) الاتصال.

```csharp
public CredentialsMethodType CredentialsMethodType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyCredentialsMethodTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // إضافة ورقة عمل وإنشاء جدول محوري لإنشاء اتصال خارجي.
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Product");
                sheet.Cells["B1"].PutValue("Sales");
                sheet.Cells["A2"].PutValue("Apple");
                sheet.Cells["B2"].PutValue(1000);
                sheet.Cells["A3"].PutValue("Banana");
                sheet.Cells["B3"].PutValue(2000);

                // إنشاء جدول محوري سيحتوي على اتصال خارجي.
                int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

                // الحصول على الاتصال الخارجي من الجدول المحوري.
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // عرض قيمة CredentialsMethodType الحالية.
                Console.WriteLine("Initial CredentialsMethodType: " + connection.CredentialsMethodType);

                // إظهار تعيين الخاصية (نظرًا لأنها قابلة للقراءة والكتابة).
                connection.CredentialsMethodType = CredentialsMethodType.Stored;
                Console.WriteLine("Updated CredentialsMethodType: " + connection.CredentialsMethodType);

                // تعيين إلى قيمة أخرى للتوضيح.
                connection.CredentialsMethodType = CredentialsMethodType.Integrated;
                Console.WriteLine("Changed CredentialsMethodType: " + connection.CredentialsMethodType);

                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("CredentialsMethodTypeDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


