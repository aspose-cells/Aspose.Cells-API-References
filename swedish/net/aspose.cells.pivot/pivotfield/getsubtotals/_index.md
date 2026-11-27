---
title: "PivotField.GetSubtotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Anger om angivet delsumma ska visas för detta pivotfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/getsubtotals/
---
## PivotField.GetSubtotals method

Anger om specificerad delsumma ska visas för detta pivotfält.

```csharp
public bool GetSubtotals(PivotFieldSubtotalType subtotalType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Delssummatyp. |

### Returvärde

Returnerar om angiven delsumma visas.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetSubtotalsWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["A4"].Value = "Electronics";
            worksheet.Cells["A5"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 500;
            worksheet.Cells["B4"].Value = 1200;
            worksheet.Cells["B5"].Value = 600;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Kontrollera om Sum-delsumma är aktiverad
                bool hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is enabled: {hasSumSubtotal}");

                // Kontrollera om Average-delsumma är aktiverad
                bool hasAvgSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal is enabled: {hasAvgSubtotal}");

                // Aktivera Sum-delsumma
                pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

                // Verifiera att Sum-delsumma nu är aktiverad
                hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"After setting, Sum subtotal is enabled: {hasSumSubtotal}");

                // Uppdatera pivottabellen för att visa ändringarna
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubtotals method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("PivotFieldMethodGetSubtotalsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


