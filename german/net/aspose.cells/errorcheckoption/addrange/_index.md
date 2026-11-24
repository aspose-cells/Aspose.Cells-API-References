---
title: "ErrorCheckOption.AddRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ErrorCheckOption-Methode. Fügt einen von dieser Einstellung beeinflussten Bereich hinzu"
type: docs
url: /de/net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Fügt einen von dieser Einstellung beeinflussten Bereich hinzu.

```csharp
public int AddRange(CellArea ca)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | CellArea | Der hinzuzufügende Bereich. |

### Rückgabewert

Der Index des hinzugefügten Bereichs in der Bereichsliste dieser Einstellung.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodAddRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
            int index = optsCollection.Add();
            ErrorCheckOption opts = optsCollection[index];
            
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            
            // Bereiche mit CellArea hinzufügen
            opts.AddRange(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 3 }); // A1:D2
            opts.AddRange(new CellArea { StartRow = 2, StartColumn = 0, EndRow = 2, EndColumn = 3 }); // A3:D3
            
            // Speichere die Arbeitsmappe
            workbook.Save("ErrorCheckOptionMethodAddRangeWithCellAreaDemo.xls");
            
            Console.WriteLine("Workbook saved with error check options.");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


