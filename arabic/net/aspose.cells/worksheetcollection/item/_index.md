---
title: "WorksheetCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تحصل على عنصر Worksheet في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

يحصل على عنصر [`Worksheet`](../../worksheet/) في الفهرس المحدد.

```csharp
public Worksheet this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // استخدام خاصية Item للوصول إلى الخلية
            Cell cell = cells[0, 0];
            cell.Formula = "=SUM(1, 2, 3)";
            
            workbook.CalculateFormula();
            Console.WriteLine("Cell value: " + cell.IntValue);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

يحصل على عنصر [`Worksheet`](../../worksheet/) بالاسم المحدد.

```csharp
public Worksheet this[string sheetName] { get; }
```

| معامل | الوصف |
| --- | --- |
| sheetName | اسم Worksheet |

### قيمة الإرجاع

العنصر بالاسم المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى أوراق العمل باستخدام خاصية Item حسب الفهرس والاسم
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            
            // الوصول إلى ورقة العمل بالاسم باستخدام خاصية Item
            Worksheet accessedSheet = workbook.Worksheets["FirstSheet"];
            
            // إضافة بيانات لتوضيح الوصول إلى ورقة العمل
            Cells cells = accessedSheet.Cells;
            cells["A1"].PutValue("Worksheet accessed successfully!");
            cells["A2"].PutValue(DateTime.Now.ToString());
            
            // إدراج عمود في الورقة الثانية
            workbook.Worksheets["SecondSheet"].Cells.InsertColumn(1);
            
            // احفظ المصنف
            workbook.Save("WorksheetCollectionItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


