---
title: "ListObject.Filter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Methode. Filtert die Tabelle"
type: docs
url: /de/net/aspose.cells.tables/listobject/filter/
---
## ListObject.Filter method

Filtere die Tabelle.

```csharp
[Obsolete("Use set ListObject.HasAutoFilter property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter Filter()
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen setzen Sie bitte die ListObject.HasAutoFilter-Eigenschaft./// Diese Eigenschaft wird 12 Monate später, seit Oktober 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectMethodFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das ListObject bereitstellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Smartphone");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Monitor");
            worksheet.Cells["B4"].PutValue(250);

            try
            {
                // Erstelle ein ListObject aus einem Datenbereich mithilfe von ListObjects.Add mit den richtigen Parametern
                int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[listObjectIndex];
                
                // Erhalte AutoFilter über die Filter-Methode
                AutoFilter autoFilter = listObject.Filter();

                // Wende einen Filter auf die Price-Spalte (Index 1) an, um Elemente ≥ 800 anzuzeigen
                autoFilter.Custom(1, FilterOperatorType.GreaterOrEqual, 800);

                Console.WriteLine("Filter applied successfully. Showing items with Price >= 800.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Filter method: {ex.Message}");
            }

            workbook.Save("ListObjectMethodFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


