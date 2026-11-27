---
title: "VbaProject.Encoding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject egenskap. Hämtar och anger kodningen för VBA-projektet"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

Hämtar och anger kodningen för VBA-projektet.

```csharp
public Encoding Encoding { get; set; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyEncodingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Initiera VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;

            // Ställ in VBA-projektets egenskaper inklusive kodning
            vbaProject.Name = "TestVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Lägg till en modul i VBA-projektet
            vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");

            // Spara arbetsboken med VBA-projekt
            workbook.Save("VbaProjectEncodingDemo.xlsm");
        }
    }
}
```

### Se även

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


