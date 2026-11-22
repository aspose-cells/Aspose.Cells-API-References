---
title: "WorksheetCollection.TableStyles"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تحصل على كائن TableStyles"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/tablestyles/
---
## WorksheetCollection.TableStyles property

يحصل على كائن `TableStyles`.

```csharp
public TableStyleCollection TableStyles { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyTableStylesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض أوراق العمل
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            
            // إنشاء وإضافة أنماط الجداول
            int styleIndex1 = workbook.Worksheets.TableStyles.AddTableStyle("Style1");
            TableStyle style1 = workbook.Worksheets.TableStyles[styleIndex1];
            
            int styleIndex2 = workbook.Worksheets.TableStyles.AddTableStyle("Style2");
            TableStyle style2 = workbook.Worksheets.TableStyles[styleIndex2];
            
            // عرض عدد أنماط الجداول
            Console.WriteLine("Table styles count: " + workbook.Worksheets.TableStyles.Count);
            
            // إزالة نمط واحد
            workbook.Worksheets.TableStyles.RemoveAt(0);
            
            // عرض العدد المحدث
            Console.WriteLine("Table styles count after removal: " + workbook.Worksheets.TableStyles.Count);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


