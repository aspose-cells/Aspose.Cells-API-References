---
title: "Name.GetRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-metod. Hämtar området om detta namn refererar till ett område"
type: docs
url: /sv/net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

Hämtar området om detta namn refererar till ett område.

```csharp
public Range GetRange()
```

### Returvärde

Området.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Skapa ett namngivet område
            int index = workbook.Worksheets.Names.Add("MyRange");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!A1:B3";
            Name namedRange = workbook.Worksheets.Names[index];
            
            // Demonstrera GetRange-metoden
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Named Range Address: " + range.Address);
            Console.WriteLine("Worksheet Name: " + range.Worksheet.Name);
            
            // Ändra området
            foreach (Cell cell in range)
            {
                if (cell.Row == 0)
                {
                    cell.PutValue(cell.StringValue.ToUpper());
                }
            }
            
            // Spara arbetsboken
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

Hämtar området om detta namn refererar till ett område

```csharp
public Range GetRange(bool recalculate)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omräkna | Boolean | om det ska omräknas om detta namn redan har beräknats före detta anrop. |

### Returvärde

Området.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll i exempeldata
            for (int i = 0; i < 4; i++)
            {
                cells[i, 1].PutValue(i); // Column B values: 0,1,2,3
            }

            // Skapa ett namngivet område med formel
            int nameIndex = wb.Worksheets.Names.Add("testname");
            Name name = wb.Worksheets.Names[nameIndex];
            name.RefersTo = "IFERROR(Sheet1!$B$2:$B$4,-1)";

            // Använd det namngivna området i formler
            cells["C1"].Formula = "=testname";
            cells["D1"].Formula = "SUM(testname)";

            // Beräkna formler
            wb.CalculateFormula();

            // Hämta området med GetRange(true)
            Aspose.Cells.Range namedRange = name.GetRange(true);
            Console.WriteLine($"Named range: FirstRow={namedRange.FirstRow}, FirstColumn={namedRange.FirstColumn}, " +
                $"RowCount={namedRange.RowCount}, ColumnCount={namedRange.ColumnCount}");

            // Skapa ett diagram med det namngivna området
            int chartIndex = sheet.Charts.Add(ChartType.Column, 10, 1, 20, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("testname", true);
            Console.WriteLine($"Chart data points count: {chart.NSeries[0].CountOfDataValues}");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

Hämtar området om detta namn refererar till ett område. Om referensen för detta namn inte är absolut kan området vara olika för olika celler.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | Det motsvarande bladindexet. |
| row | Int32 | Det motsvarande radindexet. |
| column | Int32 | Det motsvarande kolumnindexet |

### Returvärde

Området.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Dairy");
            
            // Skapa ett namngivet område med rätt metodsignatur
            int index = workbook.Worksheets.Names.Add("SubCat");
            workbook.Worksheets.Names["SubCat"].RefersTo = "=" + worksheet.Name + "!A2:A4";
            
            // Hämta område med GetRange med parametrar för rad, kolumn och radantal
            Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 0, 3);
            
            // Visa områdesreferensen
            Console.WriteLine("Range refers to: " + range.RefersTo);
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


