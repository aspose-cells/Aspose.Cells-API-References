---
title: "ExternalConnection.RefreshInternal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحدد عدد الدقائق بين عمليات التحديث التلقائي للاتصال"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/refreshinternal/
---
## ExternalConnection.RefreshInternal property

يحدد عدد الدقائق بين عمليات التحديث التلقائي للاتصال.

```csharp
public int RefreshInternal { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshInternalDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Connection Demo";
            
            try
            {
                // أنشئ اتصال بيانات (باستخدام الفئة الأساسية ExternalConnection)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // عيّن واعرض خاصية RefreshInternal
                connection.RefreshInternal = 30; // Refresh every 30 minutes
                Console.WriteLine("RefreshInternal value: " + connection.RefreshInternal);
                
                // عدّل فترة التحديث
                connection.RefreshInternal = 60;
                Console.WriteLine("Updated RefreshInternal value: " + connection.RefreshInternal);
                
                // احفظ المصنف مع إعدادات الاتصال
                workbook.Save("RefreshInternalDemo.xlsx");
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


