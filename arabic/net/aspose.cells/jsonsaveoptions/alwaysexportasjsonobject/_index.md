---
title: "JsonSaveOptions.AlwaysExportAsJsonObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonSaveOptions. تشير إلى ما إذا كان يتم دائمًا تصدير Excel إلى JSON ككائن حتى لو كان هناك ورقة عمل واحدة فقط في الملف"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

يشير إلى ما إذا كان يتم دائمًا تصدير Excel إلى JSON ككائن، حتى إذا كان هناك ورقة عمل واحدة فقط في الملف.

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyAlwaysExportAsJsonObjectDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي بورقتي عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // تعيين بعض البيانات التجريبية في ورقة العمل الأولى
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Value");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);

            // تكوين خيارات حفظ JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // احفظ إلى ملف JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);

            // عرض محتوى JSON المحفوظ
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine(jsonContent);
        }
    }
}
```

### انظر أيضًا

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


