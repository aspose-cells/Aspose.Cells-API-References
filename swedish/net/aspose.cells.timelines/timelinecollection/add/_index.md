---
title: "TimelineCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TimelineCollection-metod. Lägg till en ny Timeline med PivotTable som datakälla"
type: docs
url: /sv/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-objekt |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av Timeline-området. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av Timeline-området. |
| baseFieldName | String | Namnet på PivotField i PivotTable.BaseFields |

### Returvärde

Det nya tillagda Timeline-indexet

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 1, 3);
            cells["C4"].Value = 200;

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Column, 1);
            pivot.AddFieldToArea(PivotFieldType.Data, 2);

            // Lägg till tidslinje ansluten till pivottabellen
            sheet.Timelines.Add(pivot, 10, 5, "Date");
            
            // Spara arbetsbok
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-objekt |
| destCellName | String | Cellnamnet i det övre vänstra hörnet av Timeline-området. |
| baseFieldName | String | Namnet på PivotField i PivotTable.BaseFields |

### Returvärde

Det nya tillagda Timeline-indexet

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            
            // Lägg till pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "C1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Lägg till tidslinje ansluten till pivottabellen
            sheet.Timelines.Add(pivot, "E1", "Date");
            
            // Spara arbetsboken
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-objekt |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av Timeline-området. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av Timeline-området. |
| baseFieldIndex | Int32 | Indexet för PivotField i PivotTable.BaseFields |

### Returvärde

Det nya tillagda Timeline-indexet

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Lägg till pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till tidslinjekontroll
            sheet.Timelines.Add(pivot, 15, 5, 1);
        }
    }
}
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-objekt |
| destCellName | String | Cellnamnet i det övre vänstra hörnet av Timeline-området. |
| baseFieldIndex | Int32 | Indexet för PivotField i PivotTable.BaseFields |

### Returvärde

Det nya tillagda Timeline-indexet

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Date");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue(new DateTime(2023, 1, 1));
            cells["B2"].PutValue("A");
            cells["C2"].PutValue(100);
            
            cells["A3"].PutValue(new DateTime(2023, 1, 2));
            cells["B3"].PutValue("B");
            cells["C3"].PutValue(200);
            
            cells["A4"].PutValue(new DateTime(2023, 1, 3));
            cells["B4"].PutValue("A");
            cells["C4"].PutValue(150);

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Uppdatera pivot‑tabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Hitta basfältets index för fältet "Date"
            int dateFieldIndex = -1;
            for (int i = 0; i < pivotTable.BaseFields.Count; i++)
            {
                if (pivotTable.BaseFields[i].Name == "Date")
                {
                    dateFieldIndex = i;
                    break;
                }
            }

            // Lägg till tidslinje med det hittade indexet
            if (dateFieldIndex >= 0)
            {
                sheet.Timelines.Add(pivotTable, "H2", dateFieldIndex);
            }

            // Spara resultatet
            workbook.Save("TimelineCollectionMethodAddWithPivotTableStringInt32Demo_output.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-objekt |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av Timeline-området. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av Timeline-området. |
| baseField | PivotField | PivotField i PivotTable.BaseFields |

### Returvärde

Det nya tillagda Timeline-indexet

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 2, 1);
            cells["C4"].Value = 200;

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            
            // Lägg till pivottfält
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);
            pivot.AddFieldToArea(PivotFieldType.Column, pivot.BaseFields[1]);
            pivot.AddFieldToArea(PivotFieldType.Data, pivot.BaseFields[2]);

            // Lägg till tidslinje med pivottabellen
            sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
            
            // Spara arbetsboken
            workbook.Save("TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-objekt |
| destCellName | String | Cellnamnet i det övre vänstra hörnet av Timeline-området. |
| baseField | PivotField | PivotField i PivotTable.BaseFields |

### Returvärde

Det nya tillagda Timeline-indexet

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivot.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Lägg till tidslinje med pivottabell som datakälla
            sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[0]);
        }
    }
}
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


