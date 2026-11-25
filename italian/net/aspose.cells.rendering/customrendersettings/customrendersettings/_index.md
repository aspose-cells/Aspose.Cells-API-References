---
title: "CustomRenderSettings.CustomRenderSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore CustomRenderSettings. Ctor"
type: docs
url: /it/net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

Ctor.

```csharp
public CustomRenderSettings()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // Crea un'istanza di CustomRenderSettings usando il costruttore
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Mostra la conferma della chiamata al costruttore riuscita
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // Dimostra che l'istanza è funzionale chiamando un metodo
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // Salva la cartella di lavoro
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomRenderSettings: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


