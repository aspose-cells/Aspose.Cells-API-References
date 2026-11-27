---
title: "LowCodeLoadOptions.InputFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeLoadOptions‑egenskap. Hämtar och anger sökvägen till filen om det behövs för mallen"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodeloadoptions/inputfile/
---
## LowCodeLoadOptions.InputFile property

Hämtar och anger filen (med sökväg om behövs) för mallen.

```csharp
public string InputFile { get; set; }
```

### Anmärkningar

När du anger en icke‑null och icke‑tom sökväg för denna egenskap, kommer det tidigare angivna värdet för [`InputStream`](../inputstream/) att ignoreras.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeLoadOptionsPropertyInputFileDemo
    {
        public static void Run()
        {
            // Skapa och spara en exempelmallfil
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
            const string templatePath = "LowCodeTemplate.xlsx";
            templateWorkbook.Save(templatePath);

            // Initiera LowCodeLoadOptions och demonstrera InputFile‑egenskapen
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);

            // Ange InputFile‑egenskapen för att använda vår mall
            loadOptions.InputFile = templatePath;
            Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);

            // Läs in arbetsboken med den angivna mallfilen
            Workbook workbook = new Workbook(loadOptions.InputFile);
            
            // Modifiera den inlästa mallen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);

            // Spara den modifierade arbetsboken
            workbook.Save("PropertyInputFileDemo_Output.xlsx");
        }
    }
}
```

### Se även

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


