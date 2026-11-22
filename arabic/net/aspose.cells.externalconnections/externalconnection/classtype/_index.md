---
title: "ExternalConnection.ClassType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحصل على نوع كائن ExternalConnection هذا"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/classtype/
---
## ExternalConnection.ClassType property

تحصل على نوع هذا الكائن [`ExternalConnection`](../).

```csharp
public abstract ExternalConnectionClassType ClassType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Product {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // إنشاء جدول محوري باستخدام اتصال نموذج البيانات
            int pivotIndex = sheet.PivotTables.Add("A1:B10", "C1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // احصل على الاتصال الخارجي وعرض خاصية ClassType
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            Console.WriteLine($"Connection ClassType: {conn.ClassType}");
            Console.WriteLine($"Expected ClassType: {ExternalConnectionClassType.DataModel}");

            // احفظ المصنف
            workbook.Save("ExternalConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


