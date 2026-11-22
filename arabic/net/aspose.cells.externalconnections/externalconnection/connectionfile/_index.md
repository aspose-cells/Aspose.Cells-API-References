---
title: "ExternalConnection.ConnectionFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. يحصل على ملف الاتصال"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/connectionfile/
---
## ExternalConnection.ConnectionFile property

يحصل على ملف الاتصال.

```csharp
public virtual string ConnectionFile { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyConnectionFileDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("example.xlsx");
            ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
            
            Console.WriteLine("ConnectionFile: " + conn.ConnectionFile);
            
            workbook.Save("output.xlsx");
            
            Workbook reloadedWorkbook = new Workbook("output.xlsx");
            ExternalConnection reloadedConn = reloadedWorkbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("ConnectionFile after reload: " + reloadedConn.ConnectionFile);
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


