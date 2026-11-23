---
title: "VbaProject.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProject. Obtient et définit le nom du projet VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/name/
---
## VbaProject.Name property

Obtient et définit le nom du projet VBA.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Console.WriteLine("VBA Project Name: " + workbook.VbaProject.Name);
            workbook.Save("example.xlsx");
        }
    }
}
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


