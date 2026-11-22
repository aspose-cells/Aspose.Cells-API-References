---
title: "JsonSaveOptions.SheetIndexes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonSaveOptions. تمثل فهارس الأوراق المصدرة"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/sheetindexes/
---
## JsonSaveOptions.SheetIndexes property

يمثل فهارس الأوراق المصدرة.

```csharp
public int[] SheetIndexes { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد يحتوي على عدة أوراق
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // ملء بعض البيانات في كل ورقة
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from Sheet {i + 1}");
            }

            // إنشاء مثيل JsonSaveOptions
            JsonSaveOptions options = new JsonSaveOptions();

            // عرض SheetIndexes الحالي (null بشكل افتراضي - يصدر جميع الأوراق)
            Console.WriteLine("Current SheetIndexes: " + (options.SheetIndexes == null ? "Exporting all sheets" : string.Join(",", options.SheetIndexes)));

            // تعيين لتصدير الورقة الأولى والثالثة فقط (الفهارس 0 و 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // حفظ إلى JSON مع الأوراق المحددة
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo.json", options);

            // التحقق عن طريق تحميل JSON
            string jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo.json");
            Console.WriteLine("JSON Content:");
            Console.WriteLine(jsonContent);

            // تغيير لتصدير الورقة الثانية فقط (الفهرس 1)
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json", options);

            // التحقق من تصدير ورقة واحدة
            jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json");
            Console.WriteLine("Single Sheet JSON Content:");
            Console.WriteLine(jsonContent);
        }
    }
}
```

### انظر أيضًا

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


