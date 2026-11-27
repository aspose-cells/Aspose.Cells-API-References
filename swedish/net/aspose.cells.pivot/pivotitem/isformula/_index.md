---
title: "PivotItem.IsFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-egenskap. Anger om detta pivotelement är ett beräknat formel‑element"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/isformula/
---
## PivotItem.IsFormula property

Anger om detta pivotelement är ett beräknat formelobjekt.

```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Använd istället PivotItem.IsCalculatedItem‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hämta det första pivotelementet
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Visa det aktuella värdet för IsFormula (föråldrad egenskap)
            Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);

            // Ange ett nytt värde för IsFormula (föråldrad egenskap)
            pivotItem.IsFormula = true;

            // Visa effekten - detta skulle markera pivot item som ett formelobjekt
            Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);

            // Obs: Vid verklig användning bör du använda IsCalculatedItem istället eftersom IsFormula är föråldrad
            Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);

            // Spara resultatet
            workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


