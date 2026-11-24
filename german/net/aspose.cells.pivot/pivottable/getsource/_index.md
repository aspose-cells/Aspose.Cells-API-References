---
title: "PivotTable.GetSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Gibt die Datenquelle dieser Pivot-Tabelle zurück."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/getsource/
---
## GetSource() {#getsource}

Erhalte die Datenquelle dieser Pivot-Tabelle.

```csharp
public string[] GetSource()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ruft den Quelldatenbereich ab und zeigt ihn an.
            string[] sourceData = pivotTable.GetSource();
            Console.WriteLine("Pivot Table Source: " + sourceData[0]);
            
            // Ändern Sie die Datenquelle.
            pivotTable.ChangeDataSource(new[] { "A1:B4" });
            
            // Überprüfen Sie die geänderte Quelle.
            sourceData = pivotTable.GetSource();
            Console.WriteLine("Updated Pivot Table Source: " + sourceData[0]);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GetSource(bool) {#getsource_1}

Erhalte die Datenquelle dieser Pivot-Tabelle.

```csharp
public string[] GetSource(bool isOriginal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isOriginal | Boolean | Gibt an, ob die originale oder die angezeigte Datenquelle zurückgegeben werden soll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceWithBooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Quellendaten mit lokalem Pfad abrufen (true)
            string[] localSource = pivotTable.GetSource(true);
            Console.WriteLine("Local path source: " + localSource[0]);
            
            // Quellendaten mit vollständigem Pfad abrufen (false)
            string[] fullSource = pivotTable.GetSource(false);
            Console.WriteLine("Full path source: " + fullSource[0]);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


