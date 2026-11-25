---
title: "MsoFillFormatHelper.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormatHelper. Indica se è presente un riempimento"
type: docs
url: /it/net/aspose.cells.drawing/msofillformathelper/isvisible/
---
## MsoFillFormatHelper.IsVisible property

Indica se è presente un riempimento.

```csharp
public bool IsVisible { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'etichetta per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "IsVisible Property Demo";

            try
            {
                // Crea un'istanza di MsoFillFormatHelper usando la riflessione (senza costruttore pubblico)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visualizza il valore predefinito di IsVisible
                Console.WriteLine($"Default IsVisible: {fillHelper.IsVisible}");

                // Imposta IsVisible su true
                fillHelper.IsVisible = true;
                Console.WriteLine($"After setting to true: {fillHelper.IsVisible}");

                // Imposta IsVisible su false
                fillHelper.IsVisible = false;
                Console.WriteLine($"After setting to false: {fillHelper.IsVisible}");

                // Leggi il valore corrente di IsVisible
                bool isVisible = fillHelper.IsVisible;
                Console.WriteLine($"Current IsVisible value: {isVisible}");

                // Salva la cartella di lavoro per dimostrare l'esecuzione corretta
                workbook.Save("IsVisibleDemo.xlsx");

                Console.WriteLine("IsVisible property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during IsVisible demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


