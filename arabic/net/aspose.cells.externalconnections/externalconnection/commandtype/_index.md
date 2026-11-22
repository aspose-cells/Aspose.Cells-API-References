---
title: "ExternalConnection.CommandType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحدد نوع أمر OLE DB. 1. الاستعلام يحدد اسم مكعب 2. الاستعلام يحدد جملة SQL 3. الاستعلام يحدد اسم جدول 4. الاستعلام يحدد أن المعلومات الافتراضية قد تم تقديمها ويعتمد على الموفر كيفية تفسيرها. 5. الاستعلام يكون ضد موفر بيانات قائمة مبني على الويب"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

يحدد نوع أمر OLE DB. 1. يحدد الاستعلام اسم مكعب 2. يحدد الاستعلام بيان SQL 3. يحدد الاستعلام اسم جدول 4. يحدد الاستعلام أن المعلومات الافتراضية قد تم تقديمها، ويعتمد على المزود كيفية تفسيرها. 5. الاستعلام ضد موفر بيانات قائمة ويب.

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];

            // احصل على الاتصال الخارجي
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // أظهر خاصية CommandType
            Console.WriteLine("Original CommandType: " + conn.CommandType);
            
            // غيّر وأظهر CommandType
            conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
            Console.WriteLine("Modified CommandType: " + conn.CommandType);
            
            // احفظ المصنف
            workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


