---
title: "Cells.InsertColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Infogar en ny kolumn i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/cells/insertcolumn/
---
## InsertColumn(int, bool) {#insertcolumn_1}

Infogar en ny kolumn i kalkylbladet.

```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindex. |
| updateReference | Boolean | Anger om referenser i andra kalkylblad kommer att uppdateras. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fyll i några exempeldata i kolumn 0
            Cells cells = sheet.Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue($"Original {i}");
            }

            // Infoga en ny kolumn vid index 1 och flytta kolumner åt höger
            cells.InsertColumn(1, true);

            // Kopiera data från kolumn 0 till den nya kolumnen 1
            cells.CopyColumn(cells, 0, 1);

            // Spara arbetsboken
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumn(int) {#insertcolumn}

Infogar en ny kolumn i kalkylbladet.

```csharp
public void InsertColumn(int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hämta cellsamlingen
            Cells cells = sheet.Cells;
            
            // Infoga data i celler för demonstration
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Infoga en ny kolumn vid index 1 (kommer att bli den nya kolumnen B)
            cells.InsertColumn(1);
            
            // Verifiera genom att infoga data i den nya kolumnen
            cells["B1"].PutValue("New Column");
            
            // Spara arbetsboken
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


