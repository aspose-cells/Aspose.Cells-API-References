---
title: "Enum LookInType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LookInType Enum. Stellt den Suchtyp dar"
type: docs
url: /de/net/aspose.cells/lookintype/
---
## LookInType enumeration

Stellt den Typ 'look in' dar.

```csharp
public enum LookInType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Formulas | `0` | Findet das gesuchte Objekt aus der Formel([`Formula`](../cell/formula/)), wenn die Zelle eine Formel ist, andernfalls aus dem ursprünglichen Wert der Zelle (entspricht OriginalValues). |
| Values | `1` | Findet das Objekt aus dem ursprünglichen Wert der Zelle([`Value`](../cell/value/)) und dem formatierten Wert([`StringValue`](../cell/stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | Ignoriert Zellen, die Formeln enthalten. Für Zellen ohne Formel ist es dasselbe wie bei Values. |
| Comments | `3` | Findet das Objekt nur aus dem Kommentar der Zelle. Ignoriert Zellen, die keinen Kommentar haben. |
| OnlyFormulas | `4` | Ignoriert Zellen, die keine Formel sind. Für diese Zellen, die Formeln sind, wird das gesuchte Objekt aus der Formel ([`Formula`](../cell/formula/)) gefunden. |
| OriginalValues | `5` | Finde das Objekt nur aus dem ursprünglichen Zellwert. |
| FormattedValues | `6` | Finde das Objekt nur aus dem formatierten Zellwert ([`StringValue`](../cell/stringvalue/)). |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassLookInTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten und Formeln hinzu
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].Formula = "=A1";
            worksheet.Cells["C1"].PutValue("Contains B1");

            // Finde die Zelle, die die Formel mit "B1" enthält
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            Cell foundCell = worksheet.Cells.Find("B1", null, options);

            // Gib das Ergebnis aus
            if (foundCell != null)
            {
                Console.WriteLine($"Found cell at row: {foundCell.Row}, column: {foundCell.Column}");
                Console.WriteLine($"Cell value: {foundCell.StringValue}");
                Console.WriteLine($"Cell formula: {foundCell.Formula}");
            }
            else
            {
                Console.WriteLine("Cell not found");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


