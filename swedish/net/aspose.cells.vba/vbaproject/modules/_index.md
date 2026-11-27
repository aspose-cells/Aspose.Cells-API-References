---
title: "VbaProject.Modules"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject egenskap. Hämtar alla VbaModule-objekt"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Hämtar alla [`VbaModule`](../../vbamodule/) objekt.

```csharp
public VbaModuleCollection Modules { get; }
```

### Exempel

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
            
            // Lägg till en ny modul och hämta den med Modules-egenskapen
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            
            // Lägg till kod i modulen
            module.Codes = "Sub Test()\r\n    MsgBox \"Module demonstration\"\r\nEnd Sub";
            
            // Spara i makroaktiverat format
            workbook.Save("VbaModulesDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Se även

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


