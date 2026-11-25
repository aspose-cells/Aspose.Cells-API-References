---
title: "PictureCollection.Camera"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PictureCollection. Scatta una foto dell'intervallo"
type: docs
url: /it/net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

Cattura una foto dell'intervallo.

```csharp
public int Camera(int row, int column, string range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice di riga di questa immagine. |
| colonna | Int32 | L'indice di colonna di questa immagine. |
| intervallo | String | L'area che richiede la fotografia |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PictureCollectionMethodCameraWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per creare un intervallo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // Ottieni la raccolta Pictures dal foglio di lavoro
                PictureCollection pictures = worksheet.Pictures;

                // Chiama il metodo Camera per creare un'immagine della fotocamera
                // Parametri: row (riga in alto a sinistra), column (colonna in alto a sinistra), range (intervallo di origine)
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // Salva la cartella di lavoro
                workbook.Save("CameraDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Camera method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


