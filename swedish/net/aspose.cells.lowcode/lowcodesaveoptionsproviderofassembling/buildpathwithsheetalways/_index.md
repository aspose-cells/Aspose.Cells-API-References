---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling-egenskap. Anger om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är false, vilket innebär att när det bara finns ett blad så läggs inte bladindexet eller namnet och motsvarande prefix till i filsökvägen."
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways property

Om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns ett blad, kommer bladindex (eller namn) och motsvarande prefix inte att läggas till i filsökvägen.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med ett kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Skapa en instans av LowCodeSaveOptionsProviderOfAssembling
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            
            // Konfigurera sökvägsinställningar
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = true; // Use sheet name instead of index
            provider.SheetPrefix = "_Sheet_";
            provider.SplitPartPrefix = "_Part_";
            
            // Visa initialt egenskapsvärde
            Console.WriteLine("Initial BuildPathWithSheetAlways: " + provider.BuildPathWithSheetAlways);
            
            // Demonstrera filsökväg utan BuildPathWithSheetAlways
            string defaultPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (default): " + defaultPath);
            
            // Ställ in BuildPathWithSheetAlways till true
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine("\nAfter setting BuildPathWithSheetAlways to true: " + provider.BuildPathWithSheetAlways);
            
            // Demonstrera filsökväg med BuildPathWithSheetAlways (även med ett enda blad)
            string updatedPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (updated): " + updatedPath);
            
            // Spara arbetsboken (delningsbeteendet skulle använda leverantörens inställningar i verkliga scenarier)
            workbook.Save("BuildPathWithSheetAlwaysDemo.xlsx");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


