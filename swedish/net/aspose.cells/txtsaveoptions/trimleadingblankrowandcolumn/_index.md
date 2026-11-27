---
title: "TxtSaveOptions.TrimLeadingBlankRowAndColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions-egenskap. Anger om ledande tomma rader och kolumner ska trimmas som i MS Excel. Standard är true"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

Anger om inledande tomma rader och kolumner ska tas bort på samma sätt som i MS Excel. Standard är sant.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### Anmärkningar

Samma gäller regeln i ms excel, en rad/kolumn kommer inte att betraktas som tom om den har anpassad stil, även om den inte innehåller någon celldata. Vid sparande med LightCells-läge har detta alternativ ingen effekt. Användaren bör kontrollera utdataområdet genom implementeringen av [`LightCellsDataProvider`](../lightcellsdataprovider/) eller genom att ange [`ExportArea`](../exportarea/).

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimLeadingBlankRowAndColumnDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med några data och tomma rader/kolumner
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några data med inledande tomma rader och kolumner
            worksheet.Cells["C3"].PutValue("Data1");
            worksheet.Cells["D4"].PutValue("Data2");
            worksheet.Cells["E5"].PutValue("Data3");

            // Spara utan att trimma inledande tomrum
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            workbook.Save("output_with_blanks.csv", saveOptions);

            // Spara med trimning av inledande tomrum
            saveOptions.TrimLeadingBlankRowAndColumn = true;
            workbook.Save("output_trimmed.csv", saveOptions);

            Console.WriteLine("Files saved successfully. Compare output_with_blanks.csv and output_trimmed.csv to see the difference.");
        }
    }
}
```

### Se även

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


