---
title: "VbaModule.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaModule. Obtiene el tipo del módulo"
type: docs
url: /es/net/aspose.cells.vba/vbamodule/type/
---
## VbaModule.Type property

Obtiene el tipo del módulo.

```csharp
public VbaModuleType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo con archivo de muestra habilitado para macros
            Workbook wb = new Workbook("example.xlsm");
            
            // Acceder al proyecto VBA y a los módulos
            VbaProject vbaProject = wb.VbaProject;
            VbaModuleCollection modules = vbaProject.Modules;
            
            // Mostrar tipos y nombres de módulos
            for (int i = 0; i < modules.Count; i++)
            {
                Console.WriteLine($"Module Name: {modules[i].Name}");
                Console.WriteLine($"Module Type: {modules[i].Type}");
                Console.WriteLine();
            }
            
            wb.Save("output.xlsm");
        }
    }
}
```

### Ver también

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


