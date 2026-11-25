---
title: "CustomRenderSettings.GetCellBorderWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di CustomRenderSettings. Specifica la larghezza del bordo della cella in base al tipo di bordo"
type: docs
url: /it/net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

Specifica la larghezza del bordo della cella in base al tipo di bordo.

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderType | CellBorderType | tipo di bordo della cella |

### Valore di ritorno

larghezza del bordo della cella

### Osservazioni

Qualsiasi valore negativo verrà ignorato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodGetCellBorderWidthWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea un'istanza di CustomRenderSettings
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Chiama GetCellBorderWidth con diversi tipi di bordo
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Visualizza i risultati
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // Salva la cartella di lavoro
                workbook.Save("GetCellBorderWidthDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


