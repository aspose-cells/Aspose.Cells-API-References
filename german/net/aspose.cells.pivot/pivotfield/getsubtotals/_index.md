---
title: "PivotField.GetSubtotals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Gibt an, ob die angegebene Zwischensumme für dieses Pivot-Feld angezeigt werden soll"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/getsubtotals/
---
## PivotField.GetSubtotals method

Gibt an, ob die angegebene Zwischensumme für dieses Pivot‑Feld angezeigt werden soll.

```csharp
public bool GetSubtotals(PivotFieldSubtotalType subtotalType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Zwischensummentyp. |

### Rückgabewert

Gibt zurück, ob die angegebene Zwischensumme angezeigt wird.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
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

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hole das Pivot-Feld
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Prüfen, ob die Summen-Zwischensumme aktiviert ist
                bool hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is enabled: {hasSumSubtotal}");

                // Prüfen, ob die Durchschnitts-Zwischensumme aktiviert ist
                bool hasAvgSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal is enabled: {hasAvgSubtotal}");

                // Summen-Zwischensumme aktivieren
                pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

                // Überprüfen, dass die Summen-Zwischensumme jetzt aktiviert ist
                hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"After setting, Sum subtotal is enabled: {hasSumSubtotal}");

                // Pivot-Tabelle aktualisieren, um Änderungen anzuzeigen
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubtotals method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("PivotFieldMethodGetSubtotalsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


