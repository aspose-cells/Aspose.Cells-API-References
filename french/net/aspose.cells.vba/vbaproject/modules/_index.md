---
title: "VbaProject.Modules"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProject. Obtient tous les objets VbaModule"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Obtient tous les objets [`VbaModule`](../../vbamodule/).

```csharp
public VbaModuleCollection Modules { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyModulesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ajoutez un nouveau module et récupérez-le en utilisant la propriété Modules
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            
            // Ajoutez du code au module
            module.Codes = "Sub Test()\r\n    MsgBox \"Module demonstration\"\r\nEnd Sub";
            
            // Enregistrez au format avec macros activées
            workbook.Save("VbaModulesDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Voir aussi

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


