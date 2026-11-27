---
title: "ListObject.ConvertToRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject metod. Konvertera tabellen till område"
type: docs
url: /sv/net/aspose.cells.tables/listobject/converttorange/
---
## ConvertToRange() {#converttorange}

Konvertera tabellen till ett intervall.

```csharp
public void ConvertToRange()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("John");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Mary");
            
            // Skapa ett listobjekt
            int index = sheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = sheet.ListObjects[index];
            
            Console.WriteLine("Before conversion - ListObject exists: " + (listObject != null));
            
            // Konvertera listobjekt till område
            listObject.ConvertToRange();
            
            Console.WriteLine("After conversion - ListObjects count: " + sheet.ListObjects.Count);
            
            // Spara arbetsboken
            workbook.Save("ListObjectConversion.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ConvertToRange(TableToRangeOptions) {#converttorange_1}

Konvertera tabellen till ett intervall.

```csharp
public void ConvertToRange(TableToRangeOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | TableToRangeOptions | alternativen när tabellen konverteras till område. |

### Exempel

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
            
            // Skapa exempeldata
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
                for (int row = 1; row < 5; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Skapa tabell
            int tableIndex = worksheet.ListObjects.Add(0, 0, 4, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[0].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Konvertera tabell till område med alternativ
            TableToRangeOptions options = new TableToRangeOptions();
            options.LastRow = 4;
            table.ConvertToRange(options);

            workbook.Save("TableToRangeWithOptions.xlsx");
        }
    }
}
```

### Se även

* class [TableToRangeOptions](../../tabletorangeoptions/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


