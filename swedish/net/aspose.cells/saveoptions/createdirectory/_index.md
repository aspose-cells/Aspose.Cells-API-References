---
title: "SaveOptions.CreateDirectory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Om true och katalogen inte finns skapas katalogen automatiskt innan filen sparas"
type: docs
url: /sv/net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas.

```csharp
public bool CreateDirectory { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCreateDirectoryDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Ange sparalternativ med CreateDirectory aktiverat
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.CreateDirectory = true;

            // Spara arbetsboken till en ny katalog (kommer att skapas automatiskt)
            string outputPath = "OutputDirectory/example.xls";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved successfully with directory creation.");
        }
    }
}
```

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


