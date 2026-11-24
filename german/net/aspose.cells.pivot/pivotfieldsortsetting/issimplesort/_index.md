---
title: "PivotFieldSortSetting.IsSimpleSort"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFieldSortSetting-Eigenschaft. Gibt an, ob ein einfacher Datensortiervorgang angewendet wird"
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldsortsetting/issimplesort/
---
## PivotFieldSortSetting.IsSimpleSort property

Gibt an, ob ein einfacher Datensortiervorgang angewendet wird.

```csharp
public bool IsSimpleSort { get; set; }
```

### Hinweise

Der Standardwert ist true.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSimpleSortDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 150;
            worksheet.Cells["B6"].Value = 250;

            // Erstelle eine Pivot-Tabelle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // PivotField abrufen
            PivotField pivotField = pivotTable.RowFields[0];

            // Abrufen der Sortiereinstellung (schreibgeschütztes Property)
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Aktuellen IsSimpleSort-Wert anzeigen
            Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);

            // Hinweis: IsSimpleSort ist schreibgeschützt, daher können wir es nicht direkt setzen
            // Um das Sortieren zu demonstrieren, erstellen wir eine neue Pivot-Tabelle mit unterschiedlicher Sortierung

            // Erstelle eine weitere Pivot-Tabelle mit benutzerdefinierter Sortierung
            pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
            PivotTable pivotTable2 = pivotTables[pivotIndex];
            pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Sortiere das Pivot-Feld mit der verfügbaren Methode
            PivotField pivotField2 = pivotTable2.RowFields[0];
            pivotField2.SortBy(SortOrder.Ascending, -1);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


