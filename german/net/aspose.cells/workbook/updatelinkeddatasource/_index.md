---
title: "Workbook.UpdateLinkedDataSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Wenn dieses Workbook externe Links zu anderen Datenquellen enthält, wird Aspose.Cells versuchen, die neuesten Daten aus den angegebenen Quellen abzurufen"
type: docs
url: /de/net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

Wenn diese Arbeitsmappe externe Links zu anderen Datenquellen enthält, versucht Aspose.Cells, die neuesten Daten aus den angegebenen Quellen abzurufen.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Arbeitsmappen, die zum Aktualisieren der Daten externer Links, auf die sich dieses Workbook bezieht, verwendet werden. Die Zuordnung dieser Arbeitsmappen zu externen Links wird anhand von [`FileName`](../filename/) und [`DataSource`](../../externallink/datasource/) bestimmt. Bitte stellen Sie sicher, dass [`FileName`](../filename/) für jede Arbeitsmappe mit dem richtigen Wert angegeben wurde, damit sie mit dem entsprechenden externen Link verknüpft werden können. |

### Hinweise

Wenn für ein Workbook kein entsprechender externer Link gefunden wird, wird dieses Workbook ignoriert. Wenn Sie später eine Formel mit einem neuen externen Link festlegen, den Sie dem ignorierten Workbook zuordnen möchten, kann die Verknüpfung nicht durchgeführt werden, bis Sie diese Methode erneut mit diesen Arbeitsmappen aufrufen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodUpdateLinkedDataSourceWithWorkbookDemo
    {
        public static void Run()
        {
            // Erstelle ein Haupt‑Workbook mit externen Verweisen
            Workbook mainWorkbook = new Workbook();
            Worksheet mainSheet = mainWorkbook.Worksheets[0];
            mainSheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!A1";

            // Erstelle ein externes Workbook, das verknüpft wird
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["A1"].Value = "Updated External Value";

            try
            {
                // Rufe UpdateLinkedDataSource mit dem Array externer Workbooks auf
                mainWorkbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });

                // Formeln berechnen, um die Referenz zu aktualisieren
                mainWorkbook.CalculateFormula();

                // Zeigen Sie den aktualisierten Wert an
                Console.WriteLine("Updated value in main workbook: " + mainSheet.Cells["A1"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UpdateLinkedDataSource method: {ex.Message}");
            }

            // Ergebnis speichern
            mainWorkbook.Save("UpdateLinkedDataSourceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


