---
title: "TxtLoadOptions.HeaderColumnsCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. El número de columnas de encabezado que se repetirán en las hojas extendidas"
type: docs
url: /es/net/aspose.cells/txtloadoptions/headercolumnscount/
---
## TxtLoadOptions.HeaderColumnsCount property

La cantidad de columnas de encabezado que se repetirán en hojas extendidas.

```csharp
public int HeaderColumnsCount { get; set; }
```

### Observaciones

Las columnas de encabezado especificadas por esta propiedad se duplicarán en esas hojas extendidas. Esta propiedad solo tiene efecto cuando [`ExtendToNextSheet`](../extendtonextsheet/) es verdadero.

### Ejemplos

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderColumnsCountDemo
    {
        public static void Run()
        {
            // Crea contenido CSV de ejemplo
            string csvData = "Header1,Header2,Header3,Data1,Data2,Data3\n" +
                            "H1,H2,H3,D1,D2,D3\n" +
                            "A,B,C,D,E,F\n" +
                            "G,H,I,J,K,L";

            // Crear TxtLoadOptions con HeaderColumnsCount establecido en 3
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderColumnsCount = 3, // First 3 columns will be treated as headers
                Encoding = Encoding.UTF8
            };

            // Cargue los datos CSV en un libro de trabajo
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Demostrar columnas de encabezado (primeras 3 columnas)
                Console.WriteLine("Header Columns:");
                for (int row = 0; row < 2; row++)
                {
                    for (int col = 0; col < options.HeaderColumnsCount; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Demostrar columnas de datos (columnas restantes)
                Console.WriteLine("\nData Columns:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = options.HeaderColumnsCount; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }
            }
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


