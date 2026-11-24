---
title: "Klasse CellsFactory"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellsFactory class. Dienstprogramm zum Instanziieren von Klassen des Cells-Modells"
type: docs
url: /de/net/aspose.cells/cellsfactory/
---
## CellsFactory class

Dienstprogramm zum Instanziieren von Klassen des Cells-Modells.

```csharp
public class CellsFactory
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CellsFactory](cellsfactory/)() | Der Standardkonstruktor. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CreateStyle](../../aspose.cells/cellsfactory/createstyle/)() | Erstellt einen neuen Stil. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsFactoryDemo
    {
        public static void CellsFactoryExample()
        {
            // Erstelle eine neue Instanz von CellsFactory
            CellsFactory factory = new CellsFactory();

            // Verwende die Fabrik, um einen neuen Stil zu erstellen
            Style style = factory.CreateStyle();

            // Passe den Stil an
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            // Erstelle eine neue Arbeitsmappe und ein Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Den Stil auf eine bestimmte Zelle anwenden
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Cell");
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe in einer Datei
            workbook.Save("CellsFactoryExample.xlsx");
            workbook.Save("CellsFactoryExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


