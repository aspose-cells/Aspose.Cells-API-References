---
title: "PivotField.IsRepeatItemLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt an, ob die Beschriftungen des Feldes in der Zeilen- oder Spaltenregion wiederholt werden sollen. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Gibt an, ob die Bezeichnungen des Feldes in der Zeilen‑ oder Spaltenregion wiederholt werden sollen. Der Standardwert ist falsch.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsRepeatItemLabelsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");

            // Greifen Sie auf das Arbeitsblatt zu, das die Pivot‑Tabelle enthält
            Worksheet worksheet = workbook.Worksheets["Actual"];

            // Zugriff auf die PivotTable
            PivotTable pivotTable = worksheet.PivotTables[0];

            // Wiederholende Elementbeschriftungen für das erste Zeilenfeld aktivieren
            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            // Wiederholende Elementbeschriftungen für das erste Spaltenfeld aktivieren
            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


