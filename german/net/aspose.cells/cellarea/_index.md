---
title: "Struktur CellArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellArea Struktur. Stellt einen Zellbereich dar"
type: docs
url: /de/net/aspose.cells/cellarea/
---
## CellArea structure

Stellt einen Zellbereich dar.

```csharp
public struct CellArea : IComparable
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | Erstellt einen Zellbereich. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | Erstellt einen Zellbereich. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | Vergleicht zwei CellArea-Objekte anhand ihrer oberen linken Ecke. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | Gibt einen String zurück, der das aktuelle CellArea-Objekt darstellt. |

## Felder

| Name | Beschreibung |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | Liest oder setzt die Endspalte dieses Bereichs. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | Liest oder setzt die Endzeile dieses Bereichs. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | Liest oder setzt die Startspalte dieses Bereichs. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | Liest oder setzt die Startzeile dieses Bereichs. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellAreaDemo
    {
        public static void CellAreaExample()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B5"].PutValue(20);
            worksheet.Cells["B8"].PutValue(50);
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C7"].PutValue(15);
            worksheet.Cells["C9"].PutValue(30);

            // Zellbereich erstellen
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;

            // Fügen Sie eine bedingte Formatierungsregel zum Arbeitsblatt hinzu
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Speichere die Arbeitsmappe
            workbook.Save("CellAreaExample.xlsx");
            workbook.Save("CellAreaExample.pdf");

            // Demonstration der ToString-Methode
            Console.WriteLine(ca.ToString());

            // Demonstration der CompareTo-Methode
            CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            int comparisonResult = ca.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


