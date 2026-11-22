---
title: "CellWatch.CellName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellWatch. تحصل وتعيّن اسم الخلية"
type: docs
url: /ar/net/aspose.cells/cellwatch/cellname/
---
## CellWatch.CellName property

يحصل على اسم الخلية ويضبطه.

```csharp
public string CellName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyCellNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض مراقبات الخلايا
            worksheet.CellWatches.Add("B5");
            worksheet.CellWatches.Add("C10");
            
            // اعرض أسماء الخلايا لجميع المراقبات
            Console.WriteLine("Cell Watches:");
            foreach (CellWatch watch in worksheet.CellWatches)
            {
                Console.WriteLine(watch.CellName);
            }
            
            // أضف مراقبة جديدة واعرض اسمها
            worksheet.CellWatches.Add("A1");
            Console.WriteLine("Added new watch: " + 
                worksheet.CellWatches[worksheet.CellWatches.Count - 1].CellName);
            
            // احفظ المصنف
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


