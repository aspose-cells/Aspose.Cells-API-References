---
title: "CellsHelper.AltStartPath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsHelper. Obtiene o establece la ruta de inicio alternativa a la que se hace referencia en algunas referencias de fórmulas externas"
type: docs
url: /es/net/aspose.cells/cellshelper/altstartpath/
---
## CellsHelper.AltStartPath property

Obtiene o establece la ruta de inicio alternativa, a la que se hace referencia en algunas referencias de fórmulas externas.

```csharp
public static string AltStartPath { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyAltStartPathDemo
    {
        public static void Run()
        {
            // Establecer la ruta de inicio alternativa
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            
            // También establezca otras propiedades relevantes para la demostración
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            
            // Mostrar las rutas para demostrar el uso de la propiedad
            Console.WriteLine("Main Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            
            // Ejemplo de cómo podrían usarse estas rutas
            Console.WriteLine("\nWhen resources aren't found in main path, system will check: " + CellsHelper.AltStartPath);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


