---
title: "Klasse NoneBulletValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.NoneBulletValue Klasse. Stellt kein Aufzählungszeichen dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/nonebulletvalue/
---
## NoneBulletValue class

Stellt keine Aufzählung dar.

```csharp
public class NoneBulletValue : BulletValue
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [NoneBulletValue](nonebulletvalue/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| override [Type](../../aspose.cells.drawing.texts/nonebulletvalue/type/) { get; } | Ermittelt den Typ des Aufzählungszeichenwerts. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class NoneBulletValueDemo
    {
        public static void NoneBulletValueExample()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Text zu einer Zelle hinzufügen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text without bullet");

            // Erstelle ein TextBox, um Aufzählungseinstellungen anzuwenden
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "This is a TextBox without bullet points";

            // Erstelle eine Instanz von NoneBulletValue
            NoneBulletValue noneBulletValue = new NoneBulletValue();

            // Überprüfe den Typ des Aufzählungszeichens (sollte None sein)
            BulletType bulletType = noneBulletValue.Type;
            Console.WriteLine("Bullet Type: " + bulletType); // Output should be None

            // Speichern Sie die Arbeitsmappe, um die Änderungen zu demonstrieren
            workbook.Save("NoneBulletValueExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


