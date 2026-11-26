---
title: "FindOptions.ConvertNumericData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Obtiene o establece un valor que indica si se convierte el valor de cadena buscado a datos numéricos"
type: docs
url: /es/net/aspose.cells/findoptions/convertnumericdata/
---
## FindOptions.ConvertNumericData property

Obtiene o establece un valor que indica si se convierte el valor de la cadena buscada a datos numéricos.

```csharp
public bool ConvertNumericData { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra que incluyan valores numéricos como cadenas
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("456");
            worksheet.Cells["A3"].PutValue("01/28/2010");

            // Crear opciones de búsqueda y establecer ConvertNumericData en true
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;

            // Encontrar el valor de fecha (almacenado como cadena pero convertido a numérico durante la búsqueda)
            Cell foundCell = worksheet.Cells.Find("01/28/2010", null, options);

            // Mostrar el resultado
            if (foundCell != null)
            {
                Console.WriteLine("Found value at: " + foundCell.Name);
                Console.WriteLine("Cell value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("Value not found");
            }
        }
    }
}
```

### Ver también

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


