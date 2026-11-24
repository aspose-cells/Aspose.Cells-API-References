---
title: "MsoFillFormatHelper.SetOneColorGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormatHelper-Methode. Legt die angegebene Füllung als einfarbigen Farbverlauf fest"
type: docs
url: /de/net/aspose.cells.drawing/msofillformathelper/setonecolorgradient/
---
## MsoFillFormatHelper.SetOneColorGradient method

Setzt die angegebene Füllung auf einen Einfarbverlauf.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Farbe | Farbe | Eine Gradientfarbe. |
| Grad | Double | Der Grad des Farbverlaufs. Kann ein Wert von 0.0 (dunkel) bis 1.0 (hell) sein. |
| Stil | GradientStyleType | Gradient-Schattierungsstil. |
| Variante | Int32 | Die Gradientvariante. Kann einen Wert von 1 bis 4 haben, der einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fill Effects entspricht. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein einfaches Etikett im Blatt für den Kontext ein
            worksheet.Cells["A1"].Value = "Gradient Fill Demo";

            try
            {
                // Erstellen Sie eine Instanz von MsoFillFormatHelper mittels Reflexion (kein öffentlicher Konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Parameter für den Farbverlauf
                Color gradientColor = Color.FromArgb(255, 0, 120, 215); // a shade of blue
                double degree = 45.0;                                 // gradient angle in degrees
                GradientStyleType style = GradientStyleType.Horizontal; // horizontal gradient
                int variant = 0;                                      // variant (0 = default)

                // Wenden Sie den einfarbigen Farbverlauf an
                fillHelper.SetOneColorGradient(gradientColor, degree, style, variant);

                // Optional: Zeigen Sie, dass die Eigenschaften nach dem Aufruf gelesen werden können
                Console.WriteLine($"ForeColor after gradient: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency after gradient: {fillHelper.ForeColorTransparency}");

                // Speichern Sie die Arbeitsmappe (es wird keine visuelle Änderung sichtbar sein, weil der Helfer nicht an einer Form angehängt ist)
                workbook.Save("SetOneColorGradientDemo.xlsx");

                Console.WriteLine("SetOneColorGradient method called successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


