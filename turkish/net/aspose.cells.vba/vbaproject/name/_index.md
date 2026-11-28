---
title: "VbaProject.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject özelliği. VBA projesinin adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/name/
---
## VbaProject.Name property

VBA projesinin adını alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


