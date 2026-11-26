---
title: "Cells.PreserveString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene o establece un valor que indica si todos los valores de la hoja de cálculo se conservan como cadenas. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/cells/preservestring/
---
## Cells.PreserveString property

Obtiene o establece un valor que indica si todos los valores de la hoja de cálculo se conservan como cadenas. El valor predeterminado es false.

```csharp
public bool PreserveString { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyPreserveStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer la propiedad PreserveString en true
            cells.PreserveString = true;

            // Agregar valores de cadena a las celdas
            cells["A1"].PutValue("Preserved String 1");
            cells["B1"].PutValue("Preserved String 2");

            // Acceder a los valores (se conservarán como cadenas)
            Console.WriteLine("Cell A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + cells["B1"].StringValue);

            // Guarda el libro de trabajo
            workbook.Save("PreserveStringDemo.xlsx", SaveFormat.Xlsx);

            // Cargar el libro guardado para verificar la conservación
            Workbook loadedWorkbook = new Workbook("PreserveStringDemo.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;

            // Mostrar los valores conservados
            Console.WriteLine("\nAfter loading:");
            Console.WriteLine("Cell A1 value: " + loadedCells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + loadedCells["B1"].StringValue);

            // Demostrar la comparación de la propiedad PreserveString
            Console.WriteLine("\nPreserveString property matches: " + 
                (cells.PreserveString == loadedCells.PreserveString));
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


