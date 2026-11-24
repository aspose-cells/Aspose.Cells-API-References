---
title: "Worksheet.AdvancedFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet method. Filtert Daten anhand komplexer Kriterien."
type: docs
url: /de/net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

Filtert Daten mithilfe komplexer Kriterien.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isFilter | Boolean | Gibt an, ob die Liste vor Ort gefiltert wird. |
| listRange | String | Der Listenbereich. |
| criteriaRange | String | Der Kriterienbereich. |
| copyTo | String | Der Bereich, in den Daten kopiert werden. |
| uniqueRecordOnly | Boolean | Nur eindeutige Zeilen anzeigen oder kopieren. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAdvancedFilterWithBooleanStringStringStringBooleDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Filtern erstellen
            // Kopfzeilen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            // Kriterien
            worksheet.Cells["A2"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Category");
            worksheet.Cells["C2"].PutValue("Fruits");
            
            // Daten
            worksheet.Cells["A4"].PutValue("Apple");
            worksheet.Cells["B4"].PutValue("Fruits");
            worksheet.Cells["C4"].PutValue(2.5);
            
            worksheet.Cells["A5"].PutValue("Carrot");
            worksheet.Cells["B5"].PutValue("Vegetables");
            worksheet.Cells["C5"].PutValue(1.2);
            
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B6"].PutValue("Fruits");
            worksheet.Cells["C6"].PutValue(1.8);

            // Erweiterte Filter anwenden (Filter vor Ort, nur eindeutige Datensätze)
            worksheet.AdvancedFilter(false, "A4:C6", "A1:C2", null, true);

            // Speichere die Arbeitsmappe
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


