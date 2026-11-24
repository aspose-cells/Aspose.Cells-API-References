---
title: "PivotTable.EnableDataValueEditing"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt einen booleschen Wert an, der festlegt, ob der Benutzer die Zellen im Datenbereich der PivotTable bearbeiten darf. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/enabledatavalueediting/
---
## PivotTable.EnableDataValueEditing property

Gibt einen booleschen Wert an, der festlegt, ob der Benutzer die Zellen im Datenbereich der PivotTable bearbeiten darf. Der Standardwert ist false.

```csharp
public bool EnableDataValueEditing { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyEnableDataValueEditingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B5"].PutValue(3000);

            // Fügen Sie eine Pivot-Tabelle hinzu
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilenfeld und Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aktuellen Wert von EnableDataValueEditing anzeigen
            Console.WriteLine("Current EnableDataValueEditing value: " + pivotTable.EnableDataValueEditing);

            // Bearbeitung von Datenwerten aktivieren
            pivotTable.EnableDataValueEditing = true;

            // Daten berechnen, um die Pivot-Tabelle zu füllen
            pivotTable.CalculateData();

            // Arbeitsmappe vor dem Bearbeiten speichern
            workbook.Save("PivotTableBeforeEdit.xlsx");

            // Jetzt können wir die Datenwerte direkt in der PivotTable bearbeiten.
            // Zur Demonstration werden wir eine Zelle im Datenbereich ändern.
            Cell dataCell = worksheet.Cells["F5"]; // Assuming this is a data cell
            if (dataCell != null)
            {
                dataCell.PutValue(2500); // Modify the value
            }

            // Speichern Sie die Arbeitsmappe nach dem Bearbeiten
            workbook.Save("PivotTableAfterEdit.xlsx");

            // Deaktivieren Sie die Bearbeitung von Datenwerten
            pivotTable.EnableDataValueEditing = false;
            Console.WriteLine("EnableDataValueEditing set to: " + pivotTable.EnableDataValueEditing);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


