---
title: "VbaModule.Codes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModule-Eigenschaft. Ruft die Codes des Moduls ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.vba/vbamodule/codes/
---
## VbaModule.Codes property

Liest und schreibt die Codes des Moduls.

```csharp
public string Codes { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein VBA-Modul hinzufügen
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            Aspose.Cells.Vba.VbaModule module = workbook.VbaProject.Modules[index];
            
            // Initialen Code festlegen
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello World\"\nEnd Sub";
            
            // Den Code durch Anhängen neuer Zeilen ändern
            module.Codes = module.Codes + "\nSub AnotherMacro()\n    MsgBox \"Second Macro\"\nEnd Sub";
            
            // Speichere die Arbeitsmappe
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Siehe auch

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


