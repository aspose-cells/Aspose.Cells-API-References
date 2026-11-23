---
title: "VbaModule.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaModule. Obtient le type du module"
type: docs
url: /fr/net/aspose.cells.vba/vbamodule/type/
---
## VbaModule.Type property

Obtient le type du module.

```csharp
public VbaModuleType Type { get; }
```

### Exemples

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
            // Créez un classeur avec un fichier d'exemple activé par macro
            Workbook wb = new Workbook("example.xlsm");
            
            // Accédez au projet VBA et aux modules
            VbaProject vbaProject = wb.VbaProject;
            VbaModuleCollection modules = vbaProject.Modules;
            
            // Affichez les types et les noms des modules
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

### Voir aussi

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


