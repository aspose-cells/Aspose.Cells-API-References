---
title: "VbaProject.Modules"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Eigenschaft. Gibt alle VbaModule-Objekte zurück"
type: docs
url: /de/net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Gibt alle [`VbaModule`](../../vbamodule/) Objekte zurück.

```csharp
public VbaModuleCollection Modules { get; }
```

### Beispiele

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
            
            // Füge ein neues Modul hinzu und rufe es über die Modules‑Eigenschaft ab
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            
            // Füge Code zum Modul hinzu
            module.Codes = "Sub Test()\r\n    MsgBox \"Module demonstration\"\r\nEnd Sub";
            
            // Speichere im makrofähigen Format
            workbook.Save("VbaModulesDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Siehe auch

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


