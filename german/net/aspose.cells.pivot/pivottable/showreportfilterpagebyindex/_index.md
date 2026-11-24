---
title: "PivotTable.ShowReportFilterPageByIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Zeigt alle Berichtfilterseiten gemäß dem Positionsindex in den PageFields an"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showreportfilterpagebyindex/
---
## PivotTable.ShowReportFilterPageByIndex method

Zeige alle Berichtfilterseiten basierend auf dem Positionsindex in den PageFields an.

```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| posIndex | Int32 | Der Positionsindex in den PageFields |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("PivotTable.xlsx");
            
            // Greifen Sie auf das erste Arbeitsblatt zu, das die Pivot-Tabelle enthält
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Berichtfilterseiten nach Index (Position) des Seitenfelds anzeigen
            int pageFieldIndex = 0; // First page field
            pivotTable.ShowReportFilterPageByIndex(pageFieldIndex);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTable_ShowReportFilterPageByIndex_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


