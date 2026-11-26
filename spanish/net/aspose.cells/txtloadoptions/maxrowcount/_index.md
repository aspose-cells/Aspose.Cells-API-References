---
title: "TxtLoadOptions.MaxRowCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. El número máximo de filas que se importarán para una hoja"
type: docs
url: /es/net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

La cantidad máxima de filas que se importarán para una hoja.

```csharp
public int MaxRowCount { get; set; }
```

### Observaciones

Las filas que excedan este límite serán ignoradas o extendidas a la siguiente hoja según [`ExtendToNextSheet`](../extendtonextsheet/). Este recuento incluye las filas de encabezado ([`HeaderRowsCount`](../headerrowscount/)). El valor máximo permitido es el límite de filas del formato de archivo correspondiente, por ejemplo, para un archivo xlsx es 1048576. Si esta propiedad no se ha especificado o el valor especificado no es positivo, también se utilizará el límite máximo.

### Ejemplos

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxRowCountDemo
    {
        public static void Run()
        {
            // Crea contenido CSV de ejemplo
            string content = "Header1,Header2,Header3\n" +
                            "Data1,Data2,Data3\n" +
                            "Data4,Data5,Data6\n" +
                            "Data7,Data8,Data9\n" +
                            "Data10,Data11,Data12\n" +
                            "Data13,Data14,Data15\n" +
                            "Data16,Data17,Data18";

            // Crear TxtLoadOptions con MaxRowCount establecido en 4
            TxtLoadOptions opts = new TxtLoadOptions
            {
                MaxRowCount = 4,  // Only load first 4 rows (including header)
                HeaderRowsCount = 1  // First row is header
            };

            // Cargar el CSV en el libro de trabajo
            using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook wb = new Workbook(ms, opts);

                // Verificar que solo se cargaron 4 filas (1 encabezado + 3 filas de datos)
                Worksheet sheet = wb.Worksheets[0];
                Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
                Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
                Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
                Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
                Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");

                // Esto sería nulo ya que solo cargamos 4 filas (índice 0-3)
                if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
                {
                    Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
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


