---
title: "ListObject.ConvertToRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Methode. Konvertiert die Tabelle in einen Bereich"
type: docs
url: /de/net/aspose.cells.tables/listobject/converttorange/
---
## ConvertToRange() {#converttorange}

Konvertiert die Tabelle in einen Bereich.

```csharp
public void ConvertToRange()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodConvertToRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("John");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Mary");
            
            // Erstelle ein Listenobjekt
            int index = sheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = sheet.ListObjects[index];
            
            Console.WriteLine("Before conversion - ListObject exists: " + (listObject != null));
            
            // ListObject in Bereich konvertieren
            listObject.ConvertToRange();
            
            Console.WriteLine("After conversion - ListObjects count: " + sheet.ListObjects.Count);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ListObjectConversion.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ConvertToRange(TableToRangeOptions) {#converttorange_1}

Konvertiert die Tabelle in einen Bereich.

```csharp
public void ConvertToRange(TableToRangeOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | TableToRangeOptions | die Optionen beim Konvertieren einer Tabelle in einen Bereich. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodConvertToRangeWithTableToRangeOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle Beispieldaten
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
                for (int row = 1; row < 5; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Tabelle erstellen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 4, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[0].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Tabelle mit Optionen in Bereich konvertieren
            TableToRangeOptions options = new TableToRangeOptions();
            options.LastRow = 4;
            table.ConvertToRange(options);

            workbook.Save("TableToRangeWithOptions.xlsx");
        }
    }
}
```

### Siehe auch

* class [TableToRangeOptions](../../tabletorangeoptions/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


