---
title: "LoadOptions.ParsingPivotCachedRecords"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions‑Eigenschaft. Gibt an, ob beim Laden der Datei Pivot‑Cache‑Datensätze geparst werden. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. Der Standardwert ist false.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### Hinweise

Gilt nur für Excel Xlsx, Xltx, Xltm, Xlsm und xlsb-Datei

### Beispiele

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
            // CSV-Ladeoptionen erstellen
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            
            // Parsing von Pivot-Cache-Datensätzen aktivieren
            loadOptions.ParsingPivotCachedRecords = true;
            
            // Lade die Arbeitsmappe mit den Optionen
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "PivotData";
            
            // Pivot-Tabelle erstellen (zeigt, dass die Eigenschaft gesetzt ist)
            int pivotIndex = worksheet.PivotTables.Add("A1:C10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


