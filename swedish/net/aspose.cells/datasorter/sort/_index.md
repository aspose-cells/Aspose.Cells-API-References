---
title: "DataSorter.Sort"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter-metod. Sorterar data i området"
type: docs
url: /sv/net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Sorterar data i området.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| celler | Celler | Cellerna innehåller dataområdet. |
| startRow | Int32 | Startraden för området. |
| startColumn | Int32 | Startkolumnen för området. |
| endRow | Int32 | Slutraden för området. |
| endColumn | Int32 | Slutkolumnen för området. |

### Returvärde

de ursprungliga indexen (absolut position, till exempel kolumn A är 0, B är 1, ...) för de sorterade raderna/kolumnerna. Om inga rader/kolumner behöver flyttas av denna sorteringsoperation, returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Fyll i exempeldata
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            
            // Dölj en rad för att demonstrera sortering med dolda rader
            cells.Rows[1].IsHidden = true;
            
            // Skapa och konfigurera sortering
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Demonstrera Sort-metoden med Cells och Int32-parametrar
            sorter.Sort(cells, 0, 0, 5, 0);
            
            // Skriv ut resultat till konsolen
            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {cells[i, 0].IntValue}");
            }
            Console.WriteLine($"Is row 2 hidden? {cells.Rows[1].IsHidden}");
        }
    }
}
```

### Se även

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Sortera data i området.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| celler | Celler | Cellerna innehåller dataområdet. |
| område | CellArea | Området som behövs för sortering |

### Returvärde

de ursprungliga indexen (absolut position, till exempel kolumn A är 0, B är 1, ...) för de sorterade raderna/kolumnerna. Om inga rader/kolumner behöver flyttas av denna sorteringsoperation, returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(1995);
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["A3"].PutValue(1996);
            worksheet.Cells["B3"].PutValue(15000);
            worksheet.Cells["A4"].PutValue(1997);
            worksheet.Cells["B4"].PutValue(12000);
            worksheet.Cells["A5"].PutValue(1998);
            worksheet.Cells["B5"].PutValue(18000);

            // Skapa datasortering
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.HasHeaders = true;
            dataSorter.Key1 = 0; // Sort by first column (Year)
            dataSorter.Order1 = SortOrder.Descending;

            // Definiera sorteringsområde
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 1;

            // Utför sortering
            dataSorter.Sort(worksheet.Cells, area);

            // Spara arbetsboken
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Sortera data i intervallet.

```csharp
public int[] Sort()
```

### Returvärde

de ursprungliga indexen (absolut position, till exempel kolumn A är 0, B är 1, ...) för de sorterade raderna/kolumnerna. Om inga rader/kolumner behöver flyttas av denna sorteringsoperation, returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för sortering
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Skapa ett tabell/list-objekt
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Sortera data efter den första kolumnen
            table.AutoFilter.Sorter.Sort();

            // Spara arbetsboken
            workbook.Save("SortedData.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


