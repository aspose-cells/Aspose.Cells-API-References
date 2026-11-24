---
title: "PivotField.NonAutoSortDefault"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt an, ob ein Sortiervorgang, der auf dieses Pivotfeld angewendet wird, ein Autosortiervorgang oder ein einfacher Datensort ist."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

Gibt an, ob ein Sortiervorgang, der auf dieses Pivotfeld angewendet wird, ein Autosortiervorgang oder ein einfacher Datensort ist.

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft !PivotField.SortSetting.IsSimpleSort. Diese Methode wird 12 Monate nach September 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Greifen Sie auf das erste Arbeitsblatt und die Pivot-Tabelle zu
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Zugriff auf das erste Zeilenfeld in der Pivot‑Tabelle
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Setzen Sie die NonAutoSortDefault‑Eigenschaft auf true
            pivotField.NonAutoSortDefault = true;
            
            // Geben Sie den Eigenschaftswert aus
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


