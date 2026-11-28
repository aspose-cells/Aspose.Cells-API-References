---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetPrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfAssembling özelliği. Çalışma sayfası dizini için önek"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetPrefix property

Çalışma sayfası indeksinin öneki.

```csharp
public string SheetPrefix { get; set; }
```

### Açıklamalar

Eğer yalnızca bir çalışma sayfası varsa ve [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) false ise, bu önek ve çalışma sayfası dizini (veya adı) sonuç dosya yoluna eklenmez.

### Örnekler

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

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


