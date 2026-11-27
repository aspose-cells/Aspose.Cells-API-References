---
title: "Cells.InsertColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Infogar några kolumner i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/cells/insertcolumns/
---
## InsertColumns(int, int) {#insertcolumns}

Infogar några kolumner i kalkylbladet.

```csharp
public void InsertColumns(int columnIndex, int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindex. |
| totalColumns | Int32 | Antalet kolumner. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Infoga 3 kolumner med start från kolumnindex 1 (andra kolumnen)
            worksheet.Cells.InsertColumns(1, 3);
            
            // Lägg till exempeldata för att demonstrera de infogade kolumnerna
            worksheet.Cells["A1"].PutValue("Original Column");
            worksheet.Cells["B1"].PutValue("Inserted Column 1");
            worksheet.Cells["C1"].PutValue("Inserted Column 2");
            worksheet.Cells["D1"].PutValue("Inserted Column 3");
            worksheet.Cells["E1"].PutValue("Original Column 2");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, bool) {#insertcolumns_2}

Infogar några kolumner i kalkylbladet.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindex. |
| totalColumns | Int32 | Antalet kolumner. |
| updateReference | Boolean | Anger om referenser i andra kalkylblad kommer att uppdateras. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Infoga 3 kolumner vid kolumnindex 2 (0-baserat), flytta befintliga kolumner åt höger
            worksheet.Cells.InsertColumns(2, 3, true);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, InsertOptions) {#insertcolumns_1}

Infogar några kolumner i kalkylbladet.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, InsertOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindex. |
| totalColumns | Int32 | Antalet kolumner. |
| alternativ | InsertOptions | Alternativen för infogningsoperationen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // Skapa infogningsalternativ
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.Clear;

            // Infoga en kolumn vid index 1 (andra kolumnen)
            worksheet.Cells.InsertColumns(1, 1, options);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


