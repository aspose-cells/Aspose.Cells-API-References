---
title: "HtmlSaveOptions.SheetSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. يحصل أو يحدد الأوراق التي سيتم عرضها. القيمة الافتراضية هي جميع الأوراق الظاهرة في دفتر العمل Visible"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/sheetset/
---
## HtmlSaveOptions.SheetSet property

يحصل أو يحدد الأوراق التي سيتم عرضها. القيمة الافتراضية هي جميع الأوراق الظاهرة في دفتر العمل: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع عدة أوراق عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // اجعل ورقة واحدة مخفية للتوضيح
            workbook.Worksheets[1].IsVisible = false;

            // حدد بعض البيانات النموذجية في كل ورقة
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
            }

            // إنشاء كائن HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // عرض قيمة SheetSet الحالية (القيمة الافتراضية هي null والتي تعني جميع الأوراق الظاهرة)
            Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));

            // حدد SheetSet لتشمل فقط أوراق محددة (حسب الفهرس)
            options.SheetSet = new SheetSet(new int[] { 0, 2 });

            // احفظ إلى HTML - سيتم تضمين الأوراق المحددة فقط
            workbook.Save("HtmlWithCustomSheetSet.html", options);

            // غيّر SheetSet لتشمل فقط الأوراق الظاهرة
            options.SheetSet = SheetSet.Visible;
            workbook.Save("HtmlWithVisibleSheets.html", options);

            // غيّر SheetSet لتشمل الورقة النشطة فقط
            workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
            options.SheetSet = SheetSet.Active;
            workbook.Save("HtmlWithActiveSheet.html", options);
        }
    }
}
```

### انظر أيضًا

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


