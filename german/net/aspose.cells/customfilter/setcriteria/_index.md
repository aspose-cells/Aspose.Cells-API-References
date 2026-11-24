---
title: "CustomFilter.SetCriteria"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomFilter-Methode. Setzt die Filterkriterien"
type: docs
url: /de/net/aspose.cells/customfilter/setcriteria/
---
## CustomFilter.SetCriteria method

Setzt die Filterkriterien.

```csharp
public void SetCriteria(FilterOperatorType filterOperator, object criteria)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filterOperator | FilterOperatorType | Filteroperatortyp |
| Kriterien | Object | Wert des Filterkriteriums |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);

            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;

            try
            {
                // Wende einen benutzerdefinierten Filter an, um eine CustomFilter-Instanz zu erhalten
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Holen Sie den ersten benutzerdefinierten Filter aus der Filtersammlung
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Kriterien festlegen mit der SetCriteria-Methode
                customFilter.SetCriteria(FilterOperatorType.GreaterThan, 25);

                // Anzeigen der gesetzten Kriterien
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Speichere die Arbeitsmappe
                workbook.Save("SetCriteriaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


