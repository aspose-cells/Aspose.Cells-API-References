---
title: "VbaProject.Modules"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProject. Ottiene tutti gli oggetti VbaModule"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Ottiene tutti gli oggetti [`VbaModule`](../../vbamodule/).

```csharp
public VbaModuleCollection Modules { get; }
```

### Esempi

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
            
            // Aggiungi un nuovo modulo e ottienilo usando la proprietà Modules
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            
            // Aggiungi codice al modulo
            module.Codes = "Sub Test()\r\n    MsgBox \"Module demonstration\"\r\nEnd Sub";
            
            // Salva con formato abilitato alle macro
            workbook.Save("VbaModulesDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Vedi anche

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


