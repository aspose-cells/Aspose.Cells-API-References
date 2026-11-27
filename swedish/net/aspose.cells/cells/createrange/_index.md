---
title: "Cells.CreateRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cellmetod. Skapar ett Range-objekt från ett område av celler"
type: docs
url: /sv/net/aspose.cells/cells/createrange/
---
## CreateRange(string, string) {#createrange_3}

Skapar ett [`Range`](../../range/) objekt från ett område av celler.

```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftCell | String | Namn på övre vänstra cellen. |
| lowerRightCell | String | Namn på nedre högra cellen. |

### Returvärde

Ett [`Range`](../../range/) objekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Skapa ett område från A1 till A2
            Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
            range.Name = "MyRange";
            
            // Ange värden i området
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            
            // Använd området i en formel
            cells["B1"].Formula = "=SUM(MyRange)";
            
            // Beräkna formeln
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of MyRange (A1:A2) is: " + cells["B1"].IntValue);
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, int, int) {#createrange_1}

Skapar ett [`Range`](../../range/) objekt från ett område av celler.

```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Första raden i detta område |
| firstColumn | Int32 | Första kolumnen i detta område |
| totalRows | Int32 | Antal rader |
| totalColumns | Int32 | Antal kolumner |

### Returvärde

Ett [`Range`](../../range/) objekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa källområde (börjar på rad 2, kolumn 2 med 3 rader och 4 kolumner)
            Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);

            // Fyll källområdet med exempeldata
            for (int i = 0; i < rangeSrc.RowCount; i++)
            {
                for (int j = 0; j < rangeSrc.ColumnCount; j++)
                {
                    rangeSrc[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Skapa destinationsområde (börjar på rad 8, kolumn 0 med samma dimensioner)
            Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);

            // Kopiera värden från källan till destinationen
            rangeDest.CopyValue(rangeSrc);

            // Spara arbetsboken
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(string) {#createrange_2}

Skapar ett [`Range`](../../range/) objekt från en adress för intervallet.

```csharp
public Range CreateRange(string address)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | String | Adressen för intervallet. |

### Returvärde

Ett [`Range`](../../range/) objekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett område med hjälp av strängadress
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Fyll data i området
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Skapa ett annat område i ett nytt kalkylblad
            workbook.Worksheets.Add();
            Worksheet worksheet2 = workbook.Worksheets[1];
            Aspose.Cells.Range range2 = worksheet2.Cells.CreateRange("A1:C3");

            // Kopiera data mellan områden
            range2.Copy(range);

            // Spara arbetsboken
            workbook.Save("CreateRangeWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, bool) {#createrange}

Skapar ett [`Range`](../../range/) objekt från rader av celler eller kolumner av celler.

```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | Int32 | Första radindex eller första kolumnindex, nollbaserat. |
| nummer | Int32 | Totalt antal rader eller kolumner, ettbaserat. |
| ärVertikal | Boolean | Sant - Område skapat från kolumner av celler. Falskt - Område skapat från rader av celler. |

### Returvärde

Ett [`Range`](../../range/) objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa ett område som börjar från cell A1 (0,0) med 5 rader och 3 kolumner
            Aspose.Cells.Range range = cells.CreateRange(0, 0, true);

            // Fyll i lite data i området
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Row {i}, Col {j}");
                }
            }

            // Spara arbetsboken
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


