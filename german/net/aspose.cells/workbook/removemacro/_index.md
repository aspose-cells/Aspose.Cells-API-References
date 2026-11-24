---
title: "Workbook.RemoveMacro"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Entfernt VBA/Makro aus dieser Tabellenkalkulation"
type: docs
url: /de/net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

Entfernt VBA/Makro aus diesem Tabellenblatt.

```csharp
public void RemoveMacro()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveMacroDemo
    {
        public static void Run()
        {
            // Erstelle ein Workbook aus einer vorhandenen makroaktivierten Datei
            Workbook workbook = new Workbook("example.xlsm");

            // Entferne Makros aus dem Workbook
            workbook.RemoveMacro();
            
            // Speichere als makrofrei‑Workbook
            string noMacroPath = "NoMacro.xlsx";
            workbook.Save(noMacroPath, SaveFormat.Xlsx);

            Console.WriteLine("Macros removed successfully. File created: " + noMacroPath);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


