---
title: "Class VbaModule"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Vba.VbaModule class. Representerar modulen i VBA-projektet"
type: docs
url: /sv/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

Representerar modulen i VBA‑projektet.

```csharp
public class VbaModule
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BinaryCodes](../../aspose.cells.vba/vbamodule/binarycodes/) { get; } | Hämtar och anger de binära koderna för modulen. |
| [Codes](../../aspose.cells.vba/vbamodule/codes/) { get; set; } | Hämtar och anger koderna för modulen. |
| [Name](../../aspose.cells.vba/vbamodule/name/) { get; set; } | Hämtar och anger namnet på modulen. |
| [Type](../../aspose.cells.vba/vbamodule/type/) { get; } | Hämtar modulens typ. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleDemo
    {
        public static void VbaModuleExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Initiera VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;

            // Lägg till en ny modul
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");

            // Hämta VBA-modulen
            VbaModule vbaModule = vbaProject.Modules[index];

            // Ställ in koderna för modulen
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";

            // Sparar Excel-filen
            workbook.Save("VbaModuleExample.xlsm");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


