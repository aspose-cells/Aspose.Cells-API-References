---
title: "PivotTable.ShowMemberPropertyTips"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt einen booleschen Wert an, der festlegt, ob Mitglieder-Property-Informationen in den PivotTable-Tooltips weggelassen werden sollen."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showmemberpropertytips/
---
## PivotTable.ShowMemberPropertyTips property

Gibt einen booleschen Wert an, der festlegt, ob Member-Property-Informationen aus PivotTable-Tooltips weggelassen werden sollen.

```csharp
public bool ShowMemberPropertyTips { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowMemberPropertyTipsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aktuellen Wert von ShowMemberPropertyTips anzeigen
            Console.WriteLine("Current ShowMemberPropertyTips value: " + pivotTable.ShowMemberPropertyTips);

            // ShowMemberPropertyTips-Eigenschaft ändern
            pivotTable.ShowMemberPropertyTips = false;
            Console.WriteLine("ShowMemberPropertyTips set to: " + pivotTable.ShowMemberPropertyTips);

            // Daten berechnen und die Pivot-Tabelle aktualisieren
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTablePropertyShowMemberPropertyTipsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


