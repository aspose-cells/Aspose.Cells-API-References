---
title: "Classe CustomRenderSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.CustomRenderSettings. Rappresenta impostazioni personalizzate durante il rendering"
type: docs
url: /it/net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

Rappresenta le impostazioni personalizzate durante il rendering.

```csharp
public class CustomRenderSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | Ctor. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | Specifica la larghezza del bordo della cella in base al tipo di bordo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // Crea un'istanza di CustomRenderSettings utilizzando il costruttore predefinito
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Dimostra il metodo GetCellBorderWidth con diversi tipi di bordo
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Visualizza i risultati
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // Salva la cartella di lavoro
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("CustomRenderSettings demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CustomRenderSettings demonstration: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


