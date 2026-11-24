---
title: "PivotTable.DisplayNullString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob der PivotTable-Bericht eine benutzerdefinierte Zeichenfolge anzeigt, wenn der Wert null ist"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/displaynullstring/
---
## PivotTable.DisplayNullString property

Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text anzeigt, wenn der Wert null ist.

```csharp
public bool DisplayNullString { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayNullStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein Arbeitsblatt hinzufügen und mit Beispieldaten füllen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue(null);
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(null);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // PivotTable konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // DisplayNullString-Eigenschaft und benutzerdefinierte Nullzeichenfolge festlegen
            pivotTable.DisplayNullString = true;
            pivotTable.NullString = "N/A";
            
            // Daten berechnen und PivotTable aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableDisplayNullStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


