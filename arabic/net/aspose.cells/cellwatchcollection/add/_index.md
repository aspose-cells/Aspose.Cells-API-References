---
title: "CellWatchCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellWatchCollection. تضيف CellWatch مع صف وعمود"
type: docs
url: /ar/net/aspose.cells/cellwatchcollection/add/
---
## Add(int, int) {#add}

يضيف [`CellWatch`](../../cellwatch/) مع صف وعمود.

```csharp
public int Add(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### قيمة الإرجاع

يعيد موضع هذا العنصر في المجموعة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على CellWatchCollection من ورقة العمل
            CellWatchCollection cellWatchCollection = worksheet.CellWatches;
            
            try
            {
                // استدعِ طريقة Add مع مؤشرات الصف والعمود (Int32, Int32)
                int index = cellWatchCollection.Add(5, 3); // Adding cell at row 6, column D (0-based)
                
                Console.WriteLine($"CellWatch added at index: {index}");
                
                // تحقق من مراقبة الخلية المضافة
                CellWatch cellWatch = cellWatchCollection[index];
                Console.WriteLine($"Watching cell: {cellWatch.Row},{cellWatch.Column}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellWatchCollectionMethodAddWithInt32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

يضيف [`CellWatch`](../../cellwatch/) باسم الخلية.

```csharp
public int Add(string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض مراقبات الخلايا
            worksheet.CellWatches.Add("A1");
            worksheet.CellWatches.Add("B2");
            worksheet.CellWatches.Add("C3");
            
            // اعرض عدد مراقبات الخلايا
            Console.WriteLine("Cell Watches Count: " + worksheet.CellWatches.Count);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


