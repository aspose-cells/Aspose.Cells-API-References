---
title: "PivotTable.ShowReportFilterPage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Zeigt alle Berichtfilterseiten gemäß PivotField an, das PivotField muss sich in den PageFields befinden"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showreportfilterpage/
---
## PivotTable.ShowReportFilterPage method

Zeige alle Berichtfilterseiten basierend auf PivotField an, wobei das PivotField in den PageFields liegen muss.

```csharp
public void ShowReportFilterPage(PivotField pageField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageField | PivotField | Das PivotField-Objekt |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageWithPivotFieldDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("source.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt und die Pivot-Tabelle
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Berichtfilterseiten für jedes PageField anzeigen
            foreach (PivotField pageField in pivotTable.PageFields)
            {
                pivotTable.ShowReportFilterPage(pageField);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


