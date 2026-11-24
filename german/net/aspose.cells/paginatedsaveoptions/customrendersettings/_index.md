---
title: "PaginatedSaveOptions.CustomRenderSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt benutzerdefinierte Einstellungen während des Renderns zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/customrendersettings/
---
## PaginatedSaveOptions.CustomRenderSettings property

Liest oder legt benutzerdefinierte Einstellungen während des Renderns fest.

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "This demonstrates CustomRenderSettings property";

            try
            {
                // Erstellen Sie PdfSaveOptions, die von PaginatedSaveOptions erben
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Den aktuellen Wert von CustomRenderSettings abrufen
                CustomRenderSettings currentSettings = saveOptions.CustomRenderSettings;
                Console.WriteLine("Current CustomRenderSettings: " +
                    (currentSettings == null ? "null" : "CustomRenderSettings instance"));

                // Neue CustomRenderSettings erstellen und festlegen
                CustomRenderSettings newSettings = new CustomRenderSettings();
                saveOptions.CustomRenderSettings = newSettings;

                // Überprüfen Sie, ob die neuen Einstellungen angewendet wurden
                Console.WriteLine("New CustomRenderSettings set: " +
                    (saveOptions.CustomRenderSettings == newSettings ? "Success" : "Failed"));

                // Speichern Sie die Arbeitsmappe mit den benutzerdefinierten Render‑Einstellungen
                workbook.Save("CustomRenderSettingsDemo.pdf", saveOptions);
                Console.WriteLine("Workbook saved with CustomRenderSettings");
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

* class [CustomRenderSettings](../../../aspose.cells.rendering/customrendersettings/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


