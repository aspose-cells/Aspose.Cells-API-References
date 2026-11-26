---
title: "TxtLoadOptions.MaxColumnCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. El número máximo de columnas que se importarán para una hoja"
type: docs
url: /es/net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

La cantidad máxima de columnas que se importarán para una hoja.

```csharp
public int MaxColumnCount { get; set; }
```

### Observaciones

Las columnas que excedan este límite serán ignoradas o extendidas a la siguiente hoja según [`ExtendToNextSheet`](../extendtonextsheet/). Este recuento incluye las columnas de encabezado ([`HeaderColumnsCount`](../headercolumnscount/)). El valor máximo es el límite de columnas del formato de archivo correspondiente, por ejemplo, para un archivo xlsx es 16384. Si esta propiedad no se ha especificado o el valor especificado no es positivo, también se utilizará el límite máximo.

### Ejemplos

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxColumnCountDemo
    {
        public static void Run()
        {
            // Crea contenido CSV de ejemplo
            string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
                            "1,2,3,4,5,6,7,8,9,10,11\n" +
                            "a,b,c,d,e,f,g,h,i,j,k";

            // Crear TxtLoadOptions con MaxColumnCount establecido en 5
            TxtLoadOptions options = new TxtLoadOptions
            {
                MaxColumnCount = 5  // Only load first 5 columns
            };

            // Cargar el CSV con columnas limitadas
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Mostrar los datos cargados (solo deben estar presentes las primeras 5 columnas)
                Console.WriteLine("Data loaded with MaxColumnCount = 5:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Verificar que solo se cargaron 5 columnas
                Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
            }
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


