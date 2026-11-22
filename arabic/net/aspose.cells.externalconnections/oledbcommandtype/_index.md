---
title: "التعداد OLEDBCommandType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ExternalConnections.OLEDBCommandType. يحدد نوع أمر OLE DB"
type: docs
url: /ar/net/aspose.cells.externalconnections/oledbcommandtype/
---
## OLEDBCommandType enumeration

يحدد نوع أمر OLE DB.

```csharp
public enum OLEDBCommandType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لم يتم تحديد نوع الأمر. |
| CubeName | `1` | يحدد اسم المكعب |
| SqlStatement | `2` | يحدد عبارة SQL |
| TableName | `3` | يحدد اسم الجدول |
| DefaultInformation | `4` | يحدد أنه تم تقديم المعلومات الافتراضية، ويعتمد على الموفر كيفية تفسيرها. |
| WebBasedList | `5` | يحدد استعلامًا ضد موفر بيانات قائمة قائم على الويب. |
| TableCollection | `6` | يحدد قائمة الجداول. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassOLEDBCommandTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // احصل على الاتصال الخارجي
            ExternalConnectionCollection connections = workbook.DataConnections;
            ExternalConnection conn = connections[0];
            
            // عرض استخدام OLEDBCommandType
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command Type: " + conn.CommandType);
            Console.WriteLine("Command: " + conn.Command);
            
            // تغيير نوع الأمر وعرضه
            conn.CommandType = OLEDBCommandType.TableName;
            Console.WriteLine("\nAfter changing CommandType:");
            Console.WriteLine("Command Type: " + conn.CommandType);
            
            // احفظ المصنف
            workbook.Save("OLEDBCommandTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


