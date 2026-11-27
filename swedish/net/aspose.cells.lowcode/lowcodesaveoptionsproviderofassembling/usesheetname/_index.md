---
title: "LowCodeSaveOptionsProviderOfAssembling.UseSheetName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling-egenskap. Anger om filvägen byggs med bladnamn istället för bladindex. Standardvärde är falskt"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/
---
## LowCodeSaveOptionsProviderOfAssembling.UseSheetName property

Om filvägen byggs med bladnamn istället för bladindex. Standardvärdet är falskt.

```csharp
public bool UseSheetName { get; set; }
```

### Anmärkningar

Bladnamnet kommer aldrig att byggas om automatiskt. Så när det sätts till true, vänligen säkerställ att det inte finns något speciellt bladnamn som kan orsaka ogiltig filsökväg eller namn.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyUseSheetNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med namngivet kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "MonthlyReport";
            
            // Lägg till exempeldata för splittdemonstration
            for(int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Record {i+1}");
            }

            // Skapa och konfigurera leverantören
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "split_files/",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet_",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Demonstrera UseSheetName=false (standard)
            Console.WriteLine($"Default UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_default", provider.SaveOptionsTemplate.SaveFormat);

            // Ändra egenskap och demonstrera nytt beteende
            provider.UseSheetName = true;
            Console.WriteLine($"\nModified UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_modified", provider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'split_files' directory for output files with different naming schemes");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


