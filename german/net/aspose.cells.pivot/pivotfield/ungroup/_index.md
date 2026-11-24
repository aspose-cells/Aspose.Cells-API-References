---
title: "PivotField.Ungroup"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Gruppierung des Pivot-Feldes aufheben"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Gruppierung des Pivotfelds aufheben.

```csharp
public void Ungroup()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodUngroupDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Gruppierung des ersten Spaltenfelds aufheben
            pivotTable.ColumnFields[0].Ungroup();
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


