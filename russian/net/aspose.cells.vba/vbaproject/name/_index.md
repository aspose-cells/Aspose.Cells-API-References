---
title: "VbaProject.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProject. Получает и задает имя VBA проекта"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/name/
---
## VbaProject.Name property

Получает и задает имя проекта VBA.

```csharp
public string Name { get; set; }
```

### Примеры

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

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


