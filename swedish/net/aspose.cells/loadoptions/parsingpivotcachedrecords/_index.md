---
title: "LoadOptions.ParsingPivotCachedRecords"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Anger om pivottabellens cachade poster ska parsas vid inläsning av filen. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

Anger om pivot‑cachade poster ska parsas vid inläsning av filen. Standardvärdet är false.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### Anmärkningar

Gäller endast för Excel Xlsx, Xltx, Xltm, Xlsm och xlsb-filer

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingPivotCachedRecordsDemo
    {
        public static void Run()
        {
            // Skapa CSV-läsalternativ
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            
            // Aktivera parsning av pivottabellens cachade poster
            loadOptions.ParsingPivotCachedRecords = true;
            
            // Läs in arbetsboken med alternativen
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "PivotData";
            
            // Skapa pivottabell (visar att egenskapen är inställd)
            int pivotIndex = worksheet.PivotTables.Add("A1:C10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Spara arbetsboken
            workbook.Save("PivotTableOutput.xlsx");
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


