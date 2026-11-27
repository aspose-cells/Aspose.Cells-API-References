---
title: "LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling-metod. Hämtar sparaalternativen från vilka utdatainställningarna för den aktuella splittdelen erhålls"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions method

Hämtar sparalternativen som används för att få utdatainställningarna för den aktuella delade delen.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Sample Data for Split";

            try
            {
                // Skapa en instans av LowCodeSaveOptionsProviderOfAssembling
                var provider = new LowCodeSaveOptionsProviderOfAssembling
                {
                    PathHeader = "Output/",
                    PathTail = ".xlsx",
                    UseSheetName = true,
                    SheetPrefix = "Sheet_",
                    SplitPartPrefix = "Part_",
                    SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
                };

                // Skapa en SplitPartInfo-instans med reflection eftersom konstruktorn inte är åtkomlig
                var splitPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);

                // Anropa GetSaveOptions med SplitPartInfo-parameter
                LowCodeSaveOptions saveOptions = provider.GetSaveOptions(splitPartInfo);

                Console.WriteLine("SaveOptions created successfully");
                Console.WriteLine($"Output format: {saveOptions.SaveFormat}");

                // Spara arbetsboken (vid verklig användning skulle detta använda de genererade sparaalternativen)
                workbook.Save("GetSaveOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in GetSaveOptions demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


