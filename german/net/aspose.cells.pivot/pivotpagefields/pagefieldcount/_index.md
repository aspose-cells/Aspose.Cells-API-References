---
title: "PivotPageFields.PageFieldCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotPageFields-Eigenschaft. Gibt die Anzahl der Seitenfelder zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotpagefields/pagefieldcount/
---
## PivotPageFields.PageFieldCount property

Liefert die Anzahl der Seitenfelder.

```csharp
public int PageFieldCount { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsPropertyPageFieldCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Beispielarbeitsblätter mit Daten erstellen
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Data1";
            FillSampleData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Data2");
            FillSampleData(sheet2);

            // Ein Pivot-Blatt erstellen
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");

            // PivotPageFields-Instanz erstellen
            PivotPageFields pageFields = new PivotPageFields();

            // Seitenfelder hinzufügen, um die PageFieldCount-Eigenschaft zu demonstrieren
            pageFields.AddPageField(new string[] { "Category1", "Category2" });
            pageFields.AddPageField(new string[] { "Region1", "Region2" });

            try
            {
                // Den Wert der PageFieldCount-Eigenschaft anzeigen
                Console.WriteLine("Number of page fields: " + pageFields.PageFieldCount);

                // Identifikation für die Seitenfelder hinzufügen
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                pageFields.AddIdentify(1, new int[] { 1, 0 });

                // Überprüfen, ob die Anzahl nach dem Hinzufügen von Identifikationen unverändert bleibt
                Console.WriteLine("PageFieldCount after adding identifications: " + pageFields.PageFieldCount);

                // Pivot-Tabelle mit den Seitenfeldern erstellen
                string[] sources = { "=Data1!A1:C4", "=Data2!A1:C4" };
                pivotSheet.PivotTables.Add(sources, false, pageFields, "E3", "DemoPivot");

                // Speichere die Arbeitsmappe
                workbook.Save("PageFieldCountDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static void FillSampleData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Value");

            cells["A2"].PutValue("Category1");
            cells["B2"].PutValue("Region1");
            cells["C2"].PutValue(100);

            cells["A3"].PutValue("Category2");
            cells["B3"].PutValue("Region2");
            cells["C3"].PutValue(200);
        }
    }
}
```

### Siehe auch

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


