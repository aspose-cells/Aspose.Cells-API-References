---
title: "PivotTable.DataField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑egenskap. Hämtar ett PivotField‑objekt som representerar alla datafält i en pivottabell. Skrivrättigheten är endast läs. Det skapas bara när det finns två eller fler datafält i datasektionen. Som standard är det i radsektionen. Du kan dra det till rad‑/kolumnsektionen med metoden PivotTable.AddFieldToArea."
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Hämtar ett [`PivotField`](../../pivotfield/)‑objekt som representerar alla datafält i en pivottabell. Skrivrättigheten är endast läs. Det skapas bara när det finns två eller fler datafält i datasektionen. Som standard är det i radsektionen. Du kan dra det till rad‑/kolumnsektionen med metoden PivotTable.AddFieldToArea().

```csharp
[Obsolete("Use PivotTable.ValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotField DataField { get; }
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället egenskapen PivotTable.ValuesField. Denna metod kommer att tas bort 12 månader senare, från och med oktober 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Kom åt och ändra DataField‑egenskaper
            // Position är skrivskyddad, så vi demonstrerar andra egenskaper
            pivotTable.DataField.DisplayName = "Total Sales";
            pivotTable.DataField.NumberFormat = "#,##0";
            
            // Spara arbetsboken
            workbook.Save("PivotTableDataFieldDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


