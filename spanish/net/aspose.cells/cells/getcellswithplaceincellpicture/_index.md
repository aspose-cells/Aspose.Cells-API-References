---
title: "Cells.GetCellsWithPlaceInCellPicture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene todas las celdas que contienen una imagen incrustada"
type: docs
url: /es/net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

Obtiene todas las celdas que contienen una imagen incrustada.

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### Valor de retorno

Enumerador para enumerar todos los objetos Cell que contienen una imagen incrustada

### Observaciones

Si no hay ninguna imagen configurada como "Place in Cell" en esta hoja de cálculo, se devolverá null.

### Ejemplos

```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellsWithPlaceInCellPictureDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una imagen a la hoja de cálculo (esto no será contado por GetCellsWithPlaceInCellPicture)
            workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
            
            // Agregar una imagen incrustada a la celda B3 (esto será contado)
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
            
            // Eliminar la imagen flotante
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            // Obtener celdas con imágenes incrustadas
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            
            IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                    Console.WriteLine($"Found image in cell {cell.Name}");
                }
            }
            
            Console.WriteLine($"Total cells with embedded images: {count}");
            
            // Guardar y recargar para verificar la persistencia
            workbook.Save("output.xlsx");
            workbook = new Workbook("output.xlsx");
            
            // Verificar después de recargar
            cells = workbook.Worksheets[0].Cells;
            count = 0;
            enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                }
            }
            Console.WriteLine($"After reload - cells with embedded images: {count}");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


