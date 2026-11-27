---
title: "Cells.InsertRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Infogar flera rader i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/cells/insertrows/
---
## InsertRows(int, int, bool) {#insertrows_2}

Infogar flera rader i kalkylbladet.

```csharp
public void InsertRows(int rowIndex, int totalRows, bool updateReference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindex. |
| totalRows | Int32 | Antal rader som ska infogas. |
| updateReference | Boolean | Anger om referenser i andra kalkylblad kommer att uppdateras. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Infoga en rad på index 2 (kommer att bli den nya rad 3)
            worksheet.Cells.InsertRows(2, 1, true);
            
            // Lägg till data i den infogade raden
            worksheet.Cells["A3"].PutValue("Inserted Data");
            
            // Spara arbetsboken
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int, InsertOptions) {#insertrows_1}

Infogar flera rader i kalkylbladet.

```csharp
public void InsertRows(int rowIndex, int totalRows, InsertOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindex. |
| totalRows | Int32 | Antal rader som ska infogas. |
| alternativ | InsertOptions | Alternativ för infogningsoperationen. |

### Exempel

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Infoga 3 rader på radindex 5 med de angivna alternativen
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            workbook.Save("InsertRowsWithOptions.xlsx");
        }
    }
}
```

### Se även

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int) {#insertrows}

Infogar flera rader i kalkylbladet.

```csharp
public void InsertRows(int rowIndex, int totalRows)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindex. |
| totalRows | Int32 | Antal rader som ska infogas. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till lite exempeldata
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Data1");
            cells["B2"].PutValue("Data2");
            cells["A3"].PutValue("Data3");
            cells["B3"].PutValue("Data4");

            // Infoga 2 rader på radindex 2
            cells.InsertRows(2, 2);

            // Verifiera att de infogade raderna är tomma
            Console.WriteLine("Cell A2 value: " + cells[1, 0].Value); // Should be "Data1"
            Console.WriteLine("Cell A3 value: " + cells[2, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A4 value: " + cells[3, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A5 value: " + cells[4, 0].Value); // Should be "Data3"

            // Spara arbetsboken
            workbook.Save("InsertRowsDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


