---
title: "PivotField.IsRepeatItemLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Anger om fältets etiketter ska upprepas i rad‑ eller kolumnregionen. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Anger om etiketter för fältet ska upprepas i rad- eller kolumnregionen. Standardvärdet är false.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsRepeatItemLabelsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");

            // Kom åt kalkylbladet som innehåller pivottabellen
            Worksheet worksheet = workbook.Worksheets["Actual"];

            // Kom åt pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];

            // Aktivera upprepning av objektetiketter för första radfältet
            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            // Aktivera upprepande objektetiketter för första kolumnfältet
            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;

            // Spara den modifierade arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


