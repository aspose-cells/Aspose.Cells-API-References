---
title: "PivotTable.Format"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable metod. Formaterar markerat område i PivotTable"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/format/
---
## Format(PivotArea, Style) {#format_1}

Formaterar markerat område i PivotTable.

```csharp
public void Format(PivotArea pivotArea, Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotArea | PivotArea | Det valda pivottvisningsområdet. |
| style | Stil | Den formaterade inställningen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithPivotAreaStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["A4"].Value = "Truck";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 5000;
            worksheet.Cells["B3"].Value = 12000;
            worksheet.Cells["B4"].Value = 8000;

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Beräkna data för att fylla pivottabellen
            pivotTable.CalculateData();

            // Skapa en stil för formatering
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Skapa pivotområde för formatering
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.AxisType = PivotFieldType.Data;

            try
            {
                // Tillämpa formatering på pivotområdet
                pivotTable.Format(pivotArea, style);
                
                Console.WriteLine("Format method executed successfully with parameters (PivotArea, Style)");
                
                // Spara arbetsboken för att visa effekten
                workbook.Save("PivotTableFormatWithPivotAreaStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PivotArea](../../pivotarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(CellArea, Style) {#format}

Formaterar markerat område i PivotTable.

```csharp
public void Format(CellArea ca, Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Intervallet för cellerna. |
| style | Stil | Stilen |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithCellAreaStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Beräkna data och intervall
            pivotTable.CalculateData();
            pivotTable.CalculateRange();

            // Skapa en stil för formatering
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Definiera cellområde att formatera (datakroppsintervall)
            CellArea area = pivotTable.DataBodyRange;

            try
            {
                // Anropa Format-metoden med CellArea- och Style-parametrar
                pivotTable.Format(area, style);
                
                Console.WriteLine("PivotTable formatted successfully with parameters (CellArea, Style)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error formatting PivotTable: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("PivotTableFormatWithCellAreaStyleDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(int, int, Style) {#format_2}

Formaterar cellen i pivottabellområdet

```csharp
public void Format(int row, int column, Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex för cellen |
| column | Int32 | Kolumnindex för cellen |
| style | Stil | Stil som ska formatera cellen |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatWithInt32Int32StyleDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // Lägg till pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till fält i radområdet
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Beräkna data
            pivotTable.CalculateData();

            // Skapa en stil för formatering
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.Font.IsBold = true;

            // Formatera pivottabellens rubrikcell (rad 2, kolumn 0 i pivottabellkoordinater)
            pivotTable.Format(2, 0, style);

            // Spara arbetsboken
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


