---
title: "Cells.InsertRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells method. Infogar ett cellområde och flyttar celler enligt flyttalternativet"
type: docs
url: /sv/net/aspose.cells/cells/insertrange/
---
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}

Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | CellArea | Flyttområde. |
| shiftNumber | Int32 | Antal rader eller kolumner som ska infogas. |
| shiftType | ShiftType | Flyttceller-alternativ. |
| updateReference | Boolean | Indikerar om referenser ska uppdateras i andra kalkylblad. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i lite exempeldata
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);

            // Definiera området att infoga (rader 2‑3, kolumn A)
            CellArea area = CellArea.CreateCellArea(1, 0, 2, 0);

            // Infoga område som flyttar celler åt höger och uppdaterar referenser
            cells.InsertRange(area, 1, ShiftType.Right, true);

            // Verifiera operationen genom att kontrollera värden
            Console.WriteLine("A2 value after insert: " + cells["A2"].StringValue);
            Console.WriteLine("B2 value after insert: " + cells["B2"].StringValue);
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, ShiftType) {#insertrange}

Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet.

```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | CellArea | Flyttområde. |
| shiftType | ShiftType | Flyttceller-alternativ. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaShiftTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i lite exempeldata
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"R{row}C{col}");
                }
            }

            // Definiera cellområdet att infoga
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.EndRow = 4;
            area.StartColumn = 1;
            area.EndColumn = 3;

            // Infoga område och flytta celler nedåt
            cells.InsertRange(area, ShiftType.Down);

            // Spara arbetsboken
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, int, ShiftType) {#insertrange_1}

Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | CellArea | Flyttområde. |
| shiftNumber | Int32 | Antal rader eller kolumner som ska infogas. |
| shiftType | ShiftType | Flyttceller-alternativ. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Original Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["C1"].PutValue(200);
            
            // Definiera cellområdet att infoga (enda cellen B1)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 1;
            area.EndColumn = 1;
            
            // Infoga område som flyttar celler åt höger
            worksheet.Cells.InsertRange(area, 1, ShiftType.Right);
            
            // Spara arbetsboken
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


