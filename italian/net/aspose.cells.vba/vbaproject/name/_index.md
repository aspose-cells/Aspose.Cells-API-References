---
title: "VbaProject.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProject. Ottiene e imposta il nome del progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/name/
---
## VbaProject.Name property

Ottiene e imposta il nome del progetto VBA.

```csharp
public string Name { get; set; }
```

### Esempi

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

### Vedi anche

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


