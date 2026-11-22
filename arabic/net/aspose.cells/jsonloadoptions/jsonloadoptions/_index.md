---
title: "JsonLoadOptions.JsonLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ JsonLoadOptions. ينشئ خيارات تحميل الملف"
type: docs
url: /ar/net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

إنشاء خيارات تحميل الملف.

```csharp
public JsonLoadOptions()
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // دليل المصدر ودليل الإخراج
            string sourceDir = "SourceDir/";
            string outputDir = "OutputDir/";
            
            // إنشاء JsonLoadOptions باستخدام المنشئ
            JsonLoadOptions loadOptions = new JsonLoadOptions();
            loadOptions.KeptSchema = true;

            // تحميل ملف JSON باستخدام الخيارات
            Workbook workbook = new Workbook(sourceDir + "example.json", loadOptions);
            
            // حفظ كملف Excel
            workbook.Save(outputDir + "example.xlsx");

            // احفظ مرة أخرى إلى JSON باستخدام JsonSaveOptions
            workbook.Save(outputDir + "example_output.json", new JsonSaveOptions()
            {
                ExportNestedStructure = true,
                SkipEmptyRows = true
            });

            Console.WriteLine("JSON to Excel conversion completed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


