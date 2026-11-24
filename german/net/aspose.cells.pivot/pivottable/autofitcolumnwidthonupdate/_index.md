---
title: "PivotTable.AutofitColumnWidthOnUpdate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob die Spaltenbreite beim Update automatisch angepasst wird"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

Gibt an, ob die Spaltenbreite bei einer Aktualisierung automatisch angepasst werden soll

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Greifen Sie auf das Arbeitsblatt zu, das die Pivot‑Tabelle enthält
            Worksheet worksheet = workbook.Worksheets["PIVOT"];
            
            // Zugriff auf die PivotTable
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Automatisches Anpassen der Spaltenbreite beim Update deaktivieren
            pivotTable.AutofitColumnWidthOnUpdate = false;
            
            // Aktualisiere die Pivot-Tabelle, um Änderungen anzuwenden
            worksheet.RefreshPivotTables();
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


