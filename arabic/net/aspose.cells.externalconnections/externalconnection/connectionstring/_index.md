---
title: "ExternalConnection.ConnectionString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تُستخدم سلسلة معلومات الاتصال للاتصال بمصدر بيانات OLE DB أو ODBC"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/connectionstring/
---
## ExternalConnection.ConnectionString property

سلسلة معلومات الاتصال تُستخدم لإجراء اتصال بمصدر بيانات OLE DB أو ODBC.

```csharp
public virtual string ConnectionString { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء بيانات نموذجية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);
            
            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // احصل على اتصالات البيانات
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // اعرض سلسلة الاتصال إذا كانت موجودة
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection String: " + connections[0].ConnectionString);
            }
            
            // احفظ المصنف
            workbook.Save("PivotTableWithConnection.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


