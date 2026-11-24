---
title: "HtmlSaveOptions.EnableCssCustomProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions Eigenschaft. Optimiert die Ausgabe von html durch die Verwendung von CSS-Benutzerdefinierten Eigenschaften. Beispielsweise muss bei dem Szenario, dass es mehrere Vorkommen eines base64-Bildes mit benutzerdefinierter Eigenschaft gibt, die Bilddaten nur einmal gespeichert werden, sodass die Leistung des resultierenden html verbessert werden kann. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/enablecsscustomproperties/
---
## HtmlSaveOptions.EnableCssCustomProperties property

Optimiere die Ausgabe von HTML durch die Verwendung von CSS‑Custom‑Properties. Zum Beispiel muss bei mehreren Vorkommen desselben Base64‑Bildes das Bilddaten nur einmal gespeichert werden, wodurch die Leistung des resultierenden HTML verbessert wird. Der Standardwert ist false.

```csharp
public bool EnableCssCustomProperties { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit Formatierung hinzufügen
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;

            // Ein Bild hinzufügen, das in mehreren Zellen wiederholt wird
            int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
            Picture pic = worksheet.Pictures[imgIndex];
            pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
            pic.Width = 100;
            pic.Height = 100;

            // Das Bild an einen anderen Ort kopieren
            worksheet.Cells["D5"].PutValue("Same image reference:");
            int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
            pic2.Width = 100;
            pic2.Height = 100;

            // Erstelle eine HtmlSaveOptions-Instanz
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

            // Aktuellen Wert anzeigen
            Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);

            // Auf true setzen, um die CSS-Ausgabe zu optimieren
            htmlOptions.EnableCssCustomProperties = true;

            // Mit CSS-Optimierung speichern
            workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);

            // Auf false setzen zum Vergleich
            htmlOptions.EnableCssCustomProperties = false;
            workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);

            Console.WriteLine("Files saved with and without CSS custom properties optimization.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


