---
title: "ExternalConnection.Command"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات مزود البيانات والتي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات مزود البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات.

```csharp
public virtual string Command { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل وبعض البيانات النموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);
            
            // أنشئ نطاق جدول
            var range = worksheet.Cells.CreateRange("A1:B3");
            
            // أنشئ جدول محوري باستخدام النطاق كمصدر
            int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[index];
            
            // احصل على الاتصالات الخارجية
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // اعرض خاصية Command للاتصال
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection Command: " + connections[0].Command);
            }
            
            // احفظ المصنف
            workbook.Save("ExternalConnectionCommandDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


