---
title: "IExportObjectListener.ExportObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IExportObjectListener. Esporta un oggetto"
type: docs
url: /it/net/aspose.cells/iexportobjectlistener/exportobject/
---
## IExportObjectListener.ExportObject method

Esporta un oggetto.

```csharp
public object ExportObject(ExportObjectEvent e)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| e | ExportObjectEvent | L'evento attivato quando un oggetto deve essere esportato. |

### Valore di ritorno

Le informazioni sul risultato dell'esportazione dell'oggetto. Per l'esportazione di oggetti quando si esporta la cartella di lavoro in formato HTML, il risultato è una stringa URL per accedere all'Image salvata dal file html che contiene questo oggetto esportato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class IExportObjectListenerMethodExportObjectWithExportObjectEventDemo : IExportObjectListener
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Crea un'istanza della classe demo che implementa IExportObjectListener
            var listener = new IExportObjectListenerMethodExportObjectWithExportObjectEventDemo();

            try
            {
                // In uno scenario reale, l'ExportObjectEvent verrebbe fornito dal framework
                // Per scopi dimostrativi, chiameremo semplicemente il metodo con null
                object result = listener.ExportObject(null);

                Console.WriteLine("ExportObject method executed successfully.");
                Console.WriteLine($"Returned object type: {result?.GetType().Name ?? "null"}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportObject method: {ex.Message}");
            }

            workbook.Save("ExportObjectDemo.xlsx");
        }

        public object ExportObject(ExportObjectEvent e)
        {
            // Implementazione personalizzata per gestire l'esportazione
            if (e != null)
            {
                object source = e.GetSource();
                Console.WriteLine($"Exporting object of type: {source?.GetType().Name ?? "null"}");
            }
            else
            {
                Console.WriteLine("No export event provided (demo mode)");
            }

            // Restituisci un oggetto modificato o null per utilizzare il comportamento di esportazione predefinito
            return null;
        }
    }
}
```

### Vedi anche

* class [ExportObjectEvent](../../exportobjectevent/)
* interface [IExportObjectListener](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


