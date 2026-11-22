---
title: "ExternalConnection.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/name/
---
## ExternalConnection.Name property

يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("example.xlsm");

            foreach (ExternalConnection connection in workbook.DataConnections)
            {
                Console.WriteLine("Connection Name: " + connection.Name);
            }

            workbook.Save("output.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


