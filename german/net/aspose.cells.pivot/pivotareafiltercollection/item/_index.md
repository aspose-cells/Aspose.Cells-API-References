---
title: "PivotAreaFilterCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotAreaFilterCollection-Eigenschaft. Gibt den Filter aus der Liste anhand des Index zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotareafiltercollection/item/
---
## PivotAreaFilterCollection indexer

Liest den Filter aus der Liste anhand des Index.

```csharp
public PivotAreaFilter this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            
            // PivotTable hinzufügen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Fügt Felder zu Pivot-Bereichen hinzu.
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Bedingte Formatierung erstellen
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // Pivotbereich erstellen und Filter hinzufügen
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pcf.PivotAreas.Add(pivotArea);
            
            // Demonstriere die Verwendung der Item-Eigenschaft
            PivotAreaFilter filter = pivotArea.Filters[0];
            filter.IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotAreaFilterCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotAreaFilter](../../pivotareafilter/)
* class [PivotAreaFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


