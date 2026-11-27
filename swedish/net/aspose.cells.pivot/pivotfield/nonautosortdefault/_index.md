---
title: "PivotField.NonAutoSortDefault"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger om en sorteringsoperation som kommer att tillämpas på detta pivottfält är en autosorteringsoperation eller en enkel datasortering"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

Anger om en sorteringsoperation som kommer att tillämpas på detta pivottfält är en autosorteringsoperation eller en enkel datasortering.

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället !PivotField.SortSetting.IsSimpleSort property. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Få åtkomst till det första kalkylbladet och pivottabellen
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Åtkomst till det första radfältet i pivottabellen
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Ställ in NonAutoSortDefault-egenskapen till true
            pivotField.NonAutoSortDefault = true;
            
            // Skriv ut egenskapsvärdet
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


