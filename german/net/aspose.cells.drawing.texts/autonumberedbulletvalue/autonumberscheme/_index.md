---
title: "AutoNumberedBulletValue.AutonumberScheme"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoNumberedBulletValue-Eigenschaft. Stellt das Schema der automatischen Nummerierung dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/
---
## AutoNumberedBulletValue.AutonumberScheme property

Stellt das Schema der automatischen Nummerierung dar.

```csharp
public TextAutonumberScheme AutonumberScheme { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyAutonumberSchemeDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine neue Instanz von AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue();

                // Zeige den anfänglichen AutonumberScheme-Wert
                Console.WriteLine($"Default AutonumberScheme: {bullet.AutonumberScheme}");

                // Setze einen neuen AutonumberScheme-Wert
                bullet.AutonumberScheme = TextAutonumberScheme.RomanUcPeriod;
                Console.WriteLine($"Modified AutonumberScheme: {bullet.AutonumberScheme}");

                // Erstelle eine Arbeitsmappe, um die Aufzählung im Kontext zu demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Erstelle eine Form mit Text, die den Aufzählungsstil verwendet
                TextBox shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "Sample text with bullet formatting";


                // Hinweis: Die tatsächliche Anwendung des Aufzählungsstils auf Text würde zusätzliche API-Aufrufe erfordern
                // nicht in der Reflexion gezeigt. Wir speichern die Arbeitsmappe nur zur Demonstration.
                workbook.Save("AutonumberSchemeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [TextAutonumberScheme](../../textautonumberscheme/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


