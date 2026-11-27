---
title: "OoxmlSaveOptions.ExportCellName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OoxmlSaveOptions-egenskap. Anger om cellnamn ska exporteras till Excel2007 .xlsx .xlsm .xltx .xltm-fil. Om utdatafilen kan nås av SQL Server DTS måste detta värde vara sant. Att sätta värdet till falskt kommer kraftigt öka prestandan och minska filstorleken när stora filer skapas. Standardvärdet är sant."
type: docs
url: /sv/net/aspose.cells/ooxmlsaveoptions/exportcellname/
---
## OoxmlSaveOptions.ExportCellName property

Anger om cellnamn ska exporteras till Excel2007 .xlsx (.xlsm, .xltx, .xltm)-fil. Om utdatafilen kan nås av SQL Server DTS måste detta värde vara true. Att sätta värdet till false kommer kraftigt öka prestandan och minska filstorleken vid skapande av stora filer. Standardvärdet är true.

```csharp
public bool ExportCellName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyExportCellNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Placera lite data i cellerna
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            
            // Skapa XLSX-sparalternativ med ExportCellName aktiverat
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.ExportCellName = true;
            
            // Spara arbetsboken med exporterade cellnamn
            workbook.Save("output_with_cellnames.xlsx", saveOptions);
            
            // Skapa ytterligare sparalternativ med ExportCellName inaktiverat (standard)
            OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
            
            // Spara arbetsboken utan att cellnamn exporteras
            workbook.Save("output_without_cellnames.xlsx", saveOptions2);
        }
    }
}
```

### Se även

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


