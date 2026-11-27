---
title: "PivotField.IsValueFields"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger om detta fält representerar värdefält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/isvaluefields/
---
## PivotField.IsValueFields property

Anger om detta fält representerar värdefält.

```csharp
[Obsolete("Use PivotField.IsValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsValueFields { get; }
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd i stället PivotField.IsValuesField property. Denna metod kommer att tas bort 12 månader senare från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValueFieldsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Bike";
            worksheet.Cells["A4"].Value = "Car";
            worksheet.Cells["A5"].Value = "Car";
            worksheet.Cells["B2"].Value = "East";
            worksheet.Cells["B3"].Value = "West";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["B5"].Value = "West";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 3000;
            worksheet.Cells["C5"].Value = 4000;

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Lägg till kolumnfält
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");

            // Lägg till datafält och hämta det från DataFields-samlingen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];

            // Visa värdet för IsValueFields-egenskapen
            Console.WriteLine("IsValueFields for data field: " + dataField.IsValueFields);

            // Försök att hitta ett icke-datafält för att visa att IsValueFields är falskt
            foreach (PivotField field in pivotTable.RowFields)
            {
                Console.WriteLine("IsValueFields for row field '" + field.Name + "': " + field.IsValueFields);
            }

            // Spara resultatet
            workbook.Save("PivotFieldPropertyIsValueFieldsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


