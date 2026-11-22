---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetPrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfAssembling. بادئة لفهرس ورقة العمل"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetPrefix property

بادئة لفهرس ورقة العمل.

```csharp
public string SheetPrefix { get; set; }
```

### ملاحظات

إذا كان هناك ورقة عمل واحدة فقط وكان [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) غير صحيح، فلن تتم إضافة هذه البادئة وفهرس الورقة (أو اسمها) إلى مسار الملف الناتج.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetPrefixDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = false;

            Console.WriteLine("Current SheetPrefix: " + provider.SheetPrefix);
            
            provider.SheetPrefix = "Report_";
            Console.WriteLine("New SheetPrefix: " + provider.SheetPrefix);

            for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
            {
                string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
                Console.WriteLine($"Generated file path: {fileName}");
            }

            provider.SheetPrefix = "Data_";
            Console.WriteLine("Updated SheetPrefix: " + provider.SheetPrefix);

            for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
            {
                string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
                Console.WriteLine($"Generated file path: {fileName}");
            }
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


