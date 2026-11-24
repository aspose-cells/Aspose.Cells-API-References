---
title: "PivotTable.CopyStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Kopiert benannten Stil von einer anderen Pivot-Tabelle"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/copystyle/
---
## PivotTable.CopyStyle method

Kopiert benannten Stil von einer anderen PivotTable.

```csharp
public void CopyStyle(PivotTable pivotTable)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | PivotTable | Quell-Pivot-Tabelle. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCopyStyleWithPivotTableDemo
    {
        public static void Run()
        {
            // Erstellen Sie ein Quell-Arbeitsbuch mit Pivot-Tabelle
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Sales");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(200);
            
            // Erstellen Sie die Quell-Pivot-Tabelle (holen Sie das Pivot-Tabellenobjekt explizit)
            PivotTable sourcePivotTable = sourceSheet.PivotTables[sourceSheet.PivotTables.Add("PivotTable1", "A1:B3", "C3")];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Stil auf die Quell-Pivot-Tabelle anwenden
            sourcePivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Erstellen Sie ein Ziel-Arbeitsbuch mit Pivot-Tabelle
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Gleiche Datenstruktur hinzufügen
            destSheet.Cells["A1"].PutValue("Product");
            destSheet.Cells["B1"].PutValue("Sales");
            destSheet.Cells["A2"].PutValue("A");
            destSheet.Cells["B2"].PutValue(150);
            destSheet.Cells["A3"].PutValue("B");
            destSheet.Cells["B3"].PutValue(250);
            
            // Erstellen Sie die Ziel-Pivot-Tabelle (holen Sie das Pivot-Tabellenobjekt explizit)
            PivotTable destPivotTable = destSheet.PivotTables[destSheet.PivotTables.Add("PivotTable2", "A1:B3", "C3")];
            destPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            destPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Stil von der Quell-Pivot-Tabelle zur Ziel-Pivot-Tabelle kopieren
            destPivotTable.CopyStyle(sourcePivotTable);
            
            // Ergebnis speichern
            destWorkbook.Save("PivotTableStyleCopied.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


