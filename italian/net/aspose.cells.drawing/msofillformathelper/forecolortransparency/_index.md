---
title: "MsoFillFormatHelper.ForeColorTransparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormatHelper. Restituisce o imposta il grado di colore di primo piano del riempimento specificato come valore da 0,0 opaco a 1,0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/msofillformathelper/forecolortransparency/
---
## MsoFillFormatHelper.ForeColorTransparency property

Restituisce o imposta il grado del colore di primo piano del riempimento specificato come valore da 0.0 (opaco) a 1.0 (trasparente).

```csharp
public double ForeColorTransparency { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorTransparencyDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'etichetta per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "ForeColorTransparency Demo";

            try
            {
                // Crea un'istanza di MsoFillFormatHelper usando la riflessione (senza costruttore pubblico)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visualizza il valore predefinito di ForeColorTransparency
                Console.WriteLine($"Default ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Imposta un nuovo ForeColor e ForeColorTransparency
                fillHelper.ForeColor = Color.Blue;
                fillHelper.ForeColorTransparency = 0.5; // 50% transparency

                // Visualizza i valori aggiornati
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"Updated ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Dimostra la lettura del valore di trasparenza
                double transparency = fillHelper.ForeColorTransparency;
                Console.WriteLine($"Current transparency level: {transparency} (0.0=opaque, 1.0=clear)");

                // Salva la cartella di lavoro per dimostrare l'esecuzione corretta
                workbook.Save("ForeColorTransparencyDemo.xlsx");

                Console.WriteLine("ForeColorTransparency property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColorTransparency demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


