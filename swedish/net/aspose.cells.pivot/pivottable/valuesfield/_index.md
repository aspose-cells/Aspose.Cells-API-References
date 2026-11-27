---
title: "PivotTable.ValuesField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑egenskap. Hämtar ett PivotField‑objekt som representerar alla datafält i en pivottabell. Skrivrättigheten är endast läs. Det skapas bara när det finns två eller fler datafält i datasektionen. Som standard är det i radsektionen. Du kan dra det till rad‑/kolumnsektionen med metoden PivotTable.AddFieldToArea."
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/valuesfield/
---
## PivotTable.ValuesField property

Hämtar ett [`PivotField`](../../pivotfield/)‑objekt som representerar alla datafält i en pivottabell. Skrivrättigheten är endast läs. Det skapas bara när det finns två eller fler datafält i datasektionen. Som standard är det i radsektionen. Du kan dra det till rad‑/kolumnsektionen med metoden PivotTable.AddFieldToArea().

```csharp
public PivotField ValuesField { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyValuesFieldDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["A4"].PutValue("Product A");
            worksheet.Cells["B4"].PutValue("South");
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["A5"].PutValue("Product B");
            worksheet.Cells["B5"].PutValue("North");
            worksheet.Cells["C5"].PutValue(1200);

            try
            {
                // Skapa en pivottabell
                int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Lägg till fält i områden
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Beräkna data för att fylla pivottabellen
                pivotTable.CalculateData();

                // Åtkomst till ValuesField-egenskapen (skrivskyddad)
                PivotField valuesField = pivotTable.ValuesField;

                if (valuesField != null)
                {
                    Console.WriteLine("ValuesField Name: " + valuesField.Name);
                    Console.WriteLine("ValuesField DisplayName: " + valuesField.DisplayName);
                    Console.WriteLine("ValuesField Position: " + valuesField.Position);
                    Console.WriteLine("ValuesField RegionType: " + valuesField.RegionType);
                    Console.WriteLine("ValuesField IsValuesField: " + valuesField.IsValuesField);
                }
                else
                {
                    Console.WriteLine("ValuesField is null - no data fields in the pivot table");
                }

                // Spara arbetsboken
                workbook.Save("PivotTableValuesFieldDemo.xlsx");
                Console.WriteLine("PivotTable with ValuesField demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


