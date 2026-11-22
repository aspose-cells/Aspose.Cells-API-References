---
title: "PivotTable.ExternalConnectionDataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل على مصدر بيانات الاتصال الخارجي"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/externalconnectiondatasource/
---
## PivotTable.ExternalConnectionDataSource property

يحصل على مصدر بيانات الاتصال الخارجي.

```csharp
[Obsolete("Use PivotTable.GetSourceDataConnections() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ExternalConnection ExternalConnectionDataSource { get; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.GetSourceDataConnections(). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyExternalConnectionDataSourceDemo
    {
        public static void Run()
        {
            // إنشاء مصنف بوجود اتصال بيانات خارجي
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إنشاء بيانات نموذجية
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(2000);

            // إضافة جدول محوري
            int index = sheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // احصل على الاتصال الخارجي (خاصية للقراءة فقط)
            ExternalConnection connection = pivot.ExternalConnectionDataSource;
            
            if (connection != null)
            {
                Console.WriteLine("Pivot table connection: " + connection.Name);
            }
            else
            {
                Console.WriteLine("No external connection found");
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


