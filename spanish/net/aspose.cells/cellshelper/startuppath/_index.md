---
title: "CellsHelper.StartupPath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de CellsHelper. Obtiene o establece la ruta de inicio a la que se refieren algunas referencias de fórmulas externas"
type: docs
url: /es/net/aspose.cells/cellshelper/startuppath/
---
## CellsHelper.StartupPath property

Obtiene o establece la ruta de inicio a la que se hace referencia en algunas referencias de fórmulas externas.

```csharp
public static string StartupPath { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyStartupPathDemo
    {
        public static void Run()
        {
            // Establecer la ruta de inicio
            CellsHelper.StartupPath = "C:\\Temp\\AsposeCellsStartup";
            
            // Mostrar la ruta de inicio
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);

            // Demostrar propiedades adicionales de CellsHelper
            CellsHelper.SignificantDigits = 15;
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


