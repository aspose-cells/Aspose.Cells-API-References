---
title: "DBConnection.CommandType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DBConnection. تحدد نوع أمر OLE DB. 1. الاستعلام يحدد اسم مكعب 2. الاستعلام يحدد جملة SQL 3. الاستعلام يحدد اسم جدول 4. الاستعلام يحدد أن المعلومات الافتراضية قد تم توفيرها ويعتمد على الموفر كيفية تفسيرها. 5. الاستعلام يكون ضد موفر بيانات قائمة قائم على الويب"
type: docs
url: /ar/net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

يحدد نوع أمر OLE DB. 1. يحدد الاستعلام اسم مكعب 2. يحدد الاستعلام بيان SQL 3. يحدد الاستعلام اسم جدول 4. يحدد الاستعلام أن المعلومات الافتراضية قد تم تقديمها، ويعتمد على المزود كيفية تفسيرها. 5. الاستعلام ضد موفر بيانات قائمة ويب.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;

    public class DBConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // تهيئة دفتر عمل (فارغ أو من ملف قد يحتوي على اتصالات)
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى مجموعة الاتصالات الخارجية
                ExternalConnectionCollection connections = workbook.DataConnections;

                // العثور على أول DBConnection في المجموعة (إن وجد)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // عرض قيمة CommandType الحالية
                    Console.WriteLine("Original CommandType: " + dbConn.CommandType);

                    // توضيح ضبط CommandType (خاصية قراءة‑كتابة)
                    dbConn.CommandType = OLEDBCommandType.SqlStatement;
                    Console.WriteLine("Updated CommandType: " + dbConn.CommandType);
                }

                // حفظ دفتر العمل (حتى إذا لم يتغير) لتوضيح تدفق كامل
                workbook.Save("CommandTypeDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandTypeDemo.xlsx");
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

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


