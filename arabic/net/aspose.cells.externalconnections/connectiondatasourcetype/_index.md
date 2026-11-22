---
title: "التعداد ConnectionDataSourceType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ExternalConnections.ConnectionDataSourceType enum. يحدد نوع مصدر قاعدة البيانات الخارجية."
type: docs
url: /ar/net/aspose.cells.externalconnections/connectiondatasourcetype/
---
## ConnectionDataSourceType enumeration

يحدد نوع مصدر قاعدة البيانات الخارجية

```csharp
public enum ConnectionDataSourceType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| ODBCBasedSource | `1` | مصدر قائم على ODBC |
| DAOBasedSource | `2` | مصدر قائم على DAO |
| FileBasedDataBaseSource | `3` | مصدر قاعدة بيانات قائم على الملف |
| WebQuery | `4` | استعلام ويب |
| OLEDBBasedSource | `5` | مصدر قائم على OLE DB |
| TextBasedSource | `6` | مصدر قائم على النص |
| ADORecordSet | `7` | مجموعة سجلات ADO |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | مصدر بيانات OLE DB تم إنشاؤه بواسطة نموذج بيانات جدول البيانات. |
| DataFeedDataModel | `101` | مصدر بيانات تغذية البيانات تم إنشاؤه بواسطة نموذج بيانات جدول البيانات. |
| WorksheetDataModel | `102` | مصدر بيانات ورقة العمل تم إنشاؤه بواسطة نموذج بيانات جدول البيانات. |
| Table | `102` | مصدر بيانات ورقة العمل تم إنشاؤه بواسطة نموذج بيانات جدول البيانات. |
| TextDataModel | `103` | مصدر بيانات نصي تم إنشاؤه بواسطة نموذج بيانات جدول البيانات. |
| Unknown | `255` | مصدر بيانات نصي تم إنشاؤه بواسطة نموذج بيانات جدول البيانات. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassConnectionDataSourceTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(2000);

            // إنشاء جدول محوري باستخدام بيانات ورقة العمل
            var pivotTable = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            
            // الحصول على الاتصال وعرض ConnectionDataSourceType
            var conn = sheet.PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Class Type: " + conn.ClassType);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command: " + conn.Command);
            
            // احفظ المصنف
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


