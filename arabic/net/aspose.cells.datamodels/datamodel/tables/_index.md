---
title: "DataModel.Tables"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModel. تحصل على جميع الجداول في نموذج البيانات"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

يحصل على جميع الجداول في نموذج البيانات.

```csharp
public DataModelTableCollection Tables { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;

namespace AsposeCellsExamples
{
    public class DataModelPropertyTablesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // الوصول إلى نموذج البيانات
            DataModel dataModel = wb.DataModel;
            
            // احصل على مجموعة الجداول وعرض العدد
            Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
            
            // تحميل دفتر عمل تجريبي مع نموذج البيانات
            string sourceFile = "example.xlsb";
            if (System.IO.File.Exists(sourceFile))
            {
                Workbook sampleWorkbook = new Workbook(sourceFile);
                DataModel sampleDataModel = sampleWorkbook.DataModel;
                
                // الوصول إلى مجموعة الجداول
                DataModelTableCollection tables = sampleDataModel.Tables;
                Console.WriteLine($"Tables count in sample file: {tables.Count}");
                
                // التكرار عبر الجداول
                foreach (DataModelTable table in tables)
                {
                    Console.WriteLine($"Table name: {table.Name}");
                }
            }
            else
            {
                Console.WriteLine($"Sample file '{sourceFile}' not found. Create an Excel file with data model to see tables information.");
            }
        }
    }
}
```

### انظر أيضًا

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


