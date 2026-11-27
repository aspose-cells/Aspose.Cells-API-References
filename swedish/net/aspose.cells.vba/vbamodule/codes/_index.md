---
title: "VbaModule.Codes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModule-egenskap. Hämtar och anger koderna för modulen"
type: docs
url: /sv/net/aspose.cells.vba/vbamodule/codes/
---
## VbaModule.Codes property

Hämtar och anger koderna för modulen.

```csharp
public string Codes { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyCodesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en VBA-modul
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            Aspose.Cells.Vba.VbaModule module = workbook.VbaProject.Modules[index];
            
            // Ange initial kod
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello World\"\nEnd Sub";
            
            // Modifiera koden genom att lägga till nya rader
            module.Codes = module.Codes + "\nSub AnotherMacro()\n    MsgBox \"Second Macro\"\nEnd Sub";
            
            // Spara arbetsboken
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Se även

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


