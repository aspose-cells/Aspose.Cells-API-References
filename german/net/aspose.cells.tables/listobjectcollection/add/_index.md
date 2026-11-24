---
title: "ListObjectCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObjectCollection-Methode. Fügt ein ListObject zum Arbeitsblatt hinzu"
type: docs
url: /de/net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

Fügt ein ListObject dem Arbeitsblatt hinzu.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Startzeile des Listbereichs. |
| startColumn | Int32 | Die Startzeile des Listbereichs. |
| endRow | Int32 | Die Startzeile des Listbereichs. |
| endColumn | Int32 | Die Startzeile des Listbereichs. |
| hasHeaders | Boolean | Ob der Bereich Überschriften enthält. |

### Rückgabewert

Der Index des neuen ListObject

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten in einem Bereich füllen
            var range = worksheet.Cells.CreateRange("B3:D4");
            range.Value = new object[,]
            {
                {"Col1", "Col2", "Col3"},
                {100, 200, 300}
            };

            // ListObject mit der Add-Methode und Int32-Parametern hinzufügen
            int firstRow = range.FirstRow;
            int firstColumn = range.FirstColumn;
            int endRow = firstRow + range.RowCount - 1;
            int endColumn = firstColumn + range.ColumnCount - 1;
            worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // Summen aktivieren und Formel für eine Spalte festlegen
            worksheet.ListObjects[0].ShowTotals = true;
            worksheet.Cells["D5"].Formula = "=SUBTOTAL(109,[Col3])";

            // Speichere die Arbeitsmappe
            workbook.Save("ListObjectAddDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

Fügt ein ListObject dem Arbeitsblatt hinzu.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startCell | String | Die Startzelle des Listenbereichs. |
| endCell | String | Die Endzelle des Listenbereichs. |
| hasHeaders | Boolean | Ob der Bereich Überschriften enthält. |

### Rückgabewert

Der Index des neuen ListObject

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithStringStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten befüllen
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);

            // ListObject mit Zeichenkettenbereichsreferenzen hinzufügen
            ListObjectCollection listObjects = worksheet.ListObjects;
            listObjects.Add("A1", "B3", true);
            
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


