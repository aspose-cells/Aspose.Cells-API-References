---
title: "Worksheet.AutoFitColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Anpassar automatiskt kolumnbredden"
type: docs
url: /sv/net/aspose.cells/worksheet/autofitcolumn/
---
## AutoFitColumn(int, int, int) {#autofitcolumn_1}

Anpassar automatiskt kolumnbredden.

```csharp
public void AutoFitColumn(int columnIndex, int firstRow, int lastRow)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindex. |
| firstRow | Int32 | Första radens index. |
| lastRow | Int32 | Sista radens index. |

### Anmärkningar

Denna metod anpassar automatiskt en rad baserat på innehållet i ett cellintervall inom raden.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll celler med exempeldata som kommer att kräva justering av kolumnbredden
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["A2"].PutValue("This is a much longer piece of text that will require column width adjustment");
            worksheet.Cells["A3"].PutValue("Another long text entry to demonstrate AutoFitColumn");
            
            try
            {

                Console.WriteLine($"Column width before: {worksheet.Cells.GetColumnWidth(0)}");
                // Anropa AutoFitColumn på kolumn A (index 0) för raderna 0 till 2 (nollbaserat)
                worksheet.AutoFitColumn(0, 0, 2);
                
                Console.WriteLine("AutoFitColumn method executed successfully on column A for rows 1-3");
                
                // Visa effekten genom att visa kolumnbredden före och efter
                Console.WriteLine($"Column width after: {worksheet.Cells.GetColumnWidth(0)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumn method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("AutoFitColumnWithInt32Int32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumn(int) {#autofitcolumn}

Anpassar automatiskt kolumnbredden.

```csharp
public void AutoFitColumn(int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindex. |

### Anmärkningar

AutoFitColumn är en inexakt funktion.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler i kolumn 4 (0-baserat index)
            worksheet.Cells["D1"].PutValue("This is a test");
            worksheet.Cells["D2"].PutValue("AutoFitColumn demonstration");
            worksheet.Cells["D3"].PutValue("Aspose.Cells for .NET");
            
            // Auto-anpassa kolumn 4 (0-baserat index)
            worksheet.AutoFitColumn(3);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


