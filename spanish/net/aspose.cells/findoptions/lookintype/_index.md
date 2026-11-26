---
title: "FindOptions.LookInType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Tipo de búsqueda"
type: docs
url: /es/net/aspose.cells/findoptions/lookintype/
---
## FindOptions.LookInType property

Buscar en tipo.

```csharp
public LookInType LookInType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookInTypeDemo
    {
        public static void Run()
        {
            // Crea un libro y añade datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer valores y fórmulas en celdas
            worksheet.Cells["A1"].PutValue("SearchValue");
            worksheet.Cells["A2"].Formula = "=A1";
            worksheet.Cells["B1"].PutValue("OtherValue");

            // Crear opciones de búsqueda para buscar solo en fórmulas
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            // Buscar el valor en fórmulas
            Cell foundCell = worksheet.Cells.Find("SearchValue", null, options);

            // Mostrar el resultado
            if (foundCell != null)
            {
                Console.WriteLine($"Found at: Row {foundCell.Row}, Column {foundCell.Column}");
            }
            else
            {
                Console.WriteLine("Value not found in formulas");
            }
        }
    }
}
```

### Ver también

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


