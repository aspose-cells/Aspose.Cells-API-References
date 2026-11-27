---
title: "PivotTable.PreserveFormatting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om cellformatering PivotTableFormat bevaras när PivotTable uppdateras eller beräknas om"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

Anger om cellformatering ([`PivotTableFormat`](../../pivottableformat/)) bevaras när PivotTable uppdateras eller beräknas om.

```csharp
[Obsolete("Use PivotTable.PreserveCellFormattingOnUpdate property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PreserveFormatting { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotTable.PreserveCellFormattingOnUpdate. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("source.xlsx");
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Aktivera bevarande av formatering under uppdatering
            pivotTable.PreserveFormatting = true;
            
            // Applicera lite formatering på pivottabellens dataområde
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Formatera pivottabellens dataområde
            pivotTable.FormatAll(style);
            
            // Uppdatera och beräkna pivottabellsdata
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


