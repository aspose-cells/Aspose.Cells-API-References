---
title: "Cell.IsTableFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, ob diese Zelle Teil einer Tabellenformel ist"
type: docs
url: /de/net/aspose.cells/cell/istableformula/
---
## Cell.IsTableFormula property

Gibt an, ob diese Zelle Teil einer Tabellenformel ist.

```csharp
public bool IsTableFormula { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellPropertyIsTableFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Eine Tabelle erstellen
            int index = worksheet.ListObjects.Add(0, 0, 5, 3, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Tabellenformel zu Zelle D2 hinzufügen
            Cell cell = worksheet.Cells["D2"];
            cell.Formula = "=SUM(Table1[[#This Row],[Column1]:[Column3]])";
            
            // Prüfen, ob die Zelle eine Tabellenformel enthält
            Console.WriteLine("Is table formula: " + cell.IsTableFormula);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


