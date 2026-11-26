---
title: "VbaProject.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProject. Obtiene y establece el nombre del proyecto VBA"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/name/
---
## VbaProject.Name property

Obtiene y establece el nombre del proyecto VBA.

```csharp
public string Name { get; set; }
```

### Ejemplos

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

### Ver también

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


