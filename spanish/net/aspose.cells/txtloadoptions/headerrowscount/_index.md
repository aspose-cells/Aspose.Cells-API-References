---
title: "TxtLoadOptions.HeaderRowsCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. La cantidad de filas de encabezado que se repetirán para hojas extendidas"
type: docs
url: /es/net/aspose.cells/txtloadoptions/headerrowscount/
---
## TxtLoadOptions.HeaderRowsCount property

La cantidad de filas de encabezado que se repetirán en hojas extendidas.

```csharp
public int HeaderRowsCount { get; set; }
```

### Observaciones

Las filas de encabezado especificadas por esta propiedad se duplicarán para esas hojas extendidas. Esta propiedad solo tiene efecto cuando [`ExtendToNextSheet`](../extendtonextsheet/) es true.

### Ejemplos

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderRowsCountDemo
    {
        public static void Run()
        {
            // Crea contenido CSV de ejemplo
            string csvData = "Header1,Header2,Header3\n" +
                            "Value1,Value2,Value3\n" +
                            "Value4,Value5,Value6\n" +
                            "Value7,Value8,Value9";

            // Cree TxtLoadOptions con HeaderRowsCount establecido en 1
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderRowsCount = 1
            };

            // Cargue los datos CSV en un libro de trabajo
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);

                // Acceder a la primera hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Demuestre que la primera fila se trata como encabezado
                Console.WriteLine("Header Row:");
                for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                {
                    Console.Write(cells[0, col].StringValue + "\t");
                }
                Console.WriteLine("\n");

                // Muestre las filas de datos (omitiendo el encabezado)
                Console.WriteLine("Data Rows:");
                for (int row = 1; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
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


