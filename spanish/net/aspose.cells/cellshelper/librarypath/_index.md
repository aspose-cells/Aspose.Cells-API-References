---
title: "CellsHelper.LibraryPath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsHelper. Obtiene o establece la ruta de la biblioteca a la que hacen referencia algunas referencias de fórmulas externas"
type: docs
url: /es/net/aspose.cells/cellshelper/librarypath/
---
## CellsHelper.LibraryPath property

Obtiene o establece la ruta de la biblioteca a la que se hace referencia en algunas referencias de fórmulas externas.

```csharp
public static string LibraryPath { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyLibraryPathDemo
    {
        public static void Run()
        {
            // Establece la propiedad LibraryPath
            CellsHelper.LibraryPath = "C:\\MyLibraries\\AsposeCells";

            // Demuestra cómo obtener y usar LibraryPath
            Console.WriteLine("Current Library Path: " + CellsHelper.LibraryPath);

            // Ejemplo de uso de la ruta en una operación de archivo
            string filePath = System.IO.Path.Combine(CellsHelper.LibraryPath, "test.xlsx");
            Console.WriteLine("Would load file from: " + filePath);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


