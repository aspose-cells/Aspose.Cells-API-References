---
title: "Workbook.RemoveMacro"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Tar bort VBA/makro från detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

Tar bort VBA/makro från detta kalkylblad.

```csharp
public void RemoveMacro()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveMacroDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från en befintlig makroaktiverad fil
            Workbook workbook = new Workbook("example.xlsm");

            // Ta bort makron från arbetsboken
            workbook.RemoveMacro();
            
            // Spara som makrofri arbetsbok
            string noMacroPath = "NoMacro.xlsx";
            workbook.Save(noMacroPath, SaveFormat.Xlsx);

            Console.WriteLine("Macros removed successfully. File created: " + noMacroPath);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


