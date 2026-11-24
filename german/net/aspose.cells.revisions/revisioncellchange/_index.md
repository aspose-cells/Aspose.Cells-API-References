---
title: "Klasse RevisionCellChange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionCellChange Klasse. Stellt die Revision dar, die Zellen ändert"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellchange/
---
## RevisionCellChange class

Stellt die Revision dar, die Zellen ändert.

```csharp
public class RevisionCellChange : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CellName](../../aspose.cells.revisions/revisioncellchange/cellname/) { get; } | Ermittelt den Namen der Zelle. |
| [Column](../../aspose.cells.revisions/revisioncellchange/column/) { get; } | Liefert den Spaltenindex der Zelle. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| [IsNewFormatted](../../aspose.cells.revisions/revisioncellchange/isnewformatted/) { get; } | Gibt an, ob diese Zelle neu formatiert ist. |
| [IsOldFormatted](../../aspose.cells.revisions/revisioncellchange/isoldformatted/) { get; } | Gibt an, ob diese Zelle bereits formatiert ist. |
| [NewFormula](../../aspose.cells.revisions/revisioncellchange/newformula/) { get; } | Liest die alte Formel. |
| [NewStyle](../../aspose.cells.revisions/revisioncellchange/newstyle/) { get; } | Ruft den neuen Stil der Zelle ab. |
| [NewValue](../../aspose.cells.revisions/revisioncellchange/newvalue/) { get; } | Ruft den neuen Wert der Zelle ab. |
| [OldFormula](../../aspose.cells.revisions/revisioncellchange/oldformula/) { get; } | Liest die alte Formel. |
| [OldStyle](../../aspose.cells.revisions/revisioncellchange/oldstyle/) { get; } | Ruft den alten Stil der Zelle ab. |
| [OldValue](../../aspose.cells.revisions/revisioncellchange/oldvalue/) { get; } | Ruft den alten Wert der Zelle ab. |
| [Row](../../aspose.cells.revisions/revisioncellchange/row/) { get; } | Liefert den Zeilenindex der Zelle. |
| override [Type](../../aspose.cells.revisions/revisioncellchange/type/) { get; } | Stellt den Typ der Revision dar. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionCellChangeDemo
    {
        public static void Run()
        {
            // Erstelle Ausgabeverzeichnis, falls es nicht existiert
            string outputDir = "output/";
            System.IO.Directory.CreateDirectory(outputDir);
            
            string filePath = outputDir + "RevisionsClassRevisionCellChangeDemo_out.xlsx";

            // Erstelle die initiale Arbeitsmappe und aktiviere das Teilen
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Save(filePath, SaveFormat.Xlsx);

            // Öffne die Arbeitsmappe erneut, um nachverfolgte Änderungen vorzunehmen
            Workbook workbook2 = new Workbook(filePath);
            Worksheet sheet = workbook2.Worksheets[0];
            
            // Erste Revision: Setze Anfangswerte
            sheet.Cells["A1"].PutValue("Initial Value");
            sheet.Cells["B2"].PutValue(100);
            workbook2.Save(filePath, SaveFormat.Xlsx);
            
            // Zweite Revision: Werte ändern
            sheet.Cells["A1"].PutValue("Updated Value");
            sheet.Cells["B2"].PutValue(200);
            workbook2.Save(filePath, SaveFormat.Xlsx);

            // Lade die Arbeitsmappe, um auf Revisionsprotokolle zuzugreifen
            Workbook workbook3 = new Workbook(filePath);
            
            // Verarbeite alle Revisionsprotokolle
            foreach (RevisionLog log in workbook3.Worksheets.RevisionLogs)
            {
                foreach (Revision rev in log.Revisions)
                {
                    if (rev.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange rcc = (RevisionCellChange)rev;
                        Console.WriteLine($"Revision Type: {rev.Type}");
                        Console.WriteLine($"Cell: {rcc.CellName} (Row: {rcc.Row}, Column: {rcc.Column})");
                        Console.WriteLine($"Old Value: {rcc.OldValue ?? "null"}");
                        Console.WriteLine($"New Value: {rcc.NewValue ?? "null"}");
                        Console.WriteLine("------------------------------------");
                    }
                }
            }
        }
    }
}
```

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


