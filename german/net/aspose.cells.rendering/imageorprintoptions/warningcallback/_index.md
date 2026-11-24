---
title: "ImageOrPrintOptions.WarningCallback"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions‑Eigenschaft. Gibt den Warn‑Callback zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/warningcallback/
---
## ImageOrPrintOptions.WarningCallback property

Liest oder setzt den Warnungs-Callback.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Inhalt hinzu, der beim Rendern eine Warnung erzeugt
            worksheet.Cells["A1"].PutValue("This text uses a non-existent font");
            Style style = workbook.CreateStyle();
            style.Font.Name = "NonExistentFont";
            worksheet.Cells["A1"].SetStyle(style);

            // Erstelle eine ImageOrPrintOptions-Instanz
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Zeige den anfänglichen Wert von WarningCallback an
            Console.WriteLine("Current WarningCallback value: " + options.WarningCallback);

            // Erstelle und weise einen benutzerdefinierten Warn‑Callback zu
            var warningCallback = new RenderingWarningCallback();
            options.WarningCallback = warningCallback;

            // Erstelle SheetRender, um den Callback beim Rendern zu demonstrieren
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_image.png");

            // Überprüfe, ob Warnungen erfasst wurden
            Console.WriteLine($"Total warnings captured: {warningCallback.WarningCount}");
        }
    }

    // Benutzerdefinierte Callback‑Implementierung zur Behandlung von Render‑Warnungen
    public class RenderingWarningCallback : IWarningCallback
    {
        public int WarningCount { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            // Behandle Warnungen bei Schriftart‑Ersetzungen
            if (warningInfo.WarningType == WarningType.FontSubstitution)
            {
                Console.WriteLine($"Font substitution warning: {warningInfo.Description}");
                WarningCount++;
            }
        }
    }
}
```

### Siehe auch

* interface [IWarningCallback](../../../aspose.cells/iwarningcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


