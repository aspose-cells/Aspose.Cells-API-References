---
title: "PivotFieldGroupSettings.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFieldGroupSettings‑Eigenschaft. Gibt den Gruppentyp des Pivot‑Feldes zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldgroupsettings/type/
---
## PivotFieldGroupSettings.Type property

Gibt den Gruppentyp des Pivotfelds zurück.

```csharp
public virtual PivotFieldGroupType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            worksheet.Cells["A3"].Value = new DateTime(2023, 1, 2);
            worksheet.Cells["A4"].Value = new DateTime(2023, 1, 3);

            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
                int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "D3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Füge Felder zur Pivot-Tabelle hinzu
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

                // Zugriff auf das Zeilenfeld und Gruppierung nach Datum
                PivotField rowField = pivotTable.RowFields[0];
                rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("DateGroup", new int[] { 0, 1 }) }, true);

                // Zugriff auf die Gruppeneinstellungen des Zeilenfelds
                PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

                // Den aktuellen Wert der Type‑Eigenschaft anzeigen (schreibgeschützt)
                Console.WriteLine("Pivot Field Group Type: " + groupSettings.Type);

                // Speichere die Arbeitsmappe
                workbook.Save("PivotFieldGroupSettingsTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotFieldGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


