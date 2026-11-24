---
title: "ImageOrPrintOptions.IsCellAutoFit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions‑Eigenschaft. Gibt an, ob Breite und Höhe der Zellen automatisch an den Zellenwert angepasst werden. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/iscellautofit/
---
## ImageOrPrintOptions.IsCellAutoFit property

Gibt an, ob die Breite und Höhe der Zellen automatisch anhand des Zellenwerts angepasst wird. Der Standardwert ist false.

```csharp
[Obsolete("This property is not used, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCellAutoFit { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen wird diese Eigenschaft nicht verwendet, bitte entfernen Sie diese Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit August 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsCellAutoFitDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieltext festlegen, der die Standardspaltenbreite überschreitet
            worksheet.Cells["B4"].Value = "This is a long text that demonstrates cell autofit behavior when converting to image.";
            
            // Bildrenderoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Demonstration von IsCellAutoFit false (Standard)
            Console.WriteLine("Default IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithoutAutoFit.png");

            // Ändern Sie IsCellAutoFit zu true
            options.IsCellAutoFit = true;
            Console.WriteLine("Modified IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithAutoFit.png");

            Console.WriteLine("Images created successfully. Compare column widths in output files.");
        }

        private static void SaveAsImage(Worksheet worksheet, ImageOrPrintOptions options, string fileName)
        {
            // Bildformat konfigurieren
            options.ImageType = ImageType.Png;

            // Arbeitsblatt mit angegebenen Optionen in ein Bild rendern
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, fileName);
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


