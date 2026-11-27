---
title: "Worksheet.AutoFitRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Arbetsbladmetod. Anpassar automatiskt radhöjden i ett rektangulärt intervall"
type: docs
url: /sv/net/aspose.cells/worksheet/autofitrow/
---
## AutoFitRow(int, int, int, int) {#autofitrow_3}

Anpassar automatiskt radhöjden i ett rektangulärt område.

```csharp
public void AutoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradindex. |
| endRow | Int32 | Slutradindex. |
| startColumn | Int32 | Startkolumnindex. |
| endColumn | Int32 | Slutkolumnindex. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            RowCollection rows = worksheet.Cells.Rows;
            rows[0].Height = 20;
            rows[1].Height = 20;
            // Lägg till exempeldata i celler för att demonstrera automatisk radjustering
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row autofit");
            worksheet.Cells["B1"].PutValue("Additional column with text");
            worksheet.Cells["A2"].PutValue("Shorter text");
            worksheet.Cells["B2"].PutValue("More text");
            
            try
            {
                Console.WriteLine($"Row 1 height before autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height before autofit: {worksheet.Cells.Rows[1].Height}");

                // Anropa AutoFitRow med parametrarna: startRow, endRow, startColumn, endColumn
                worksheet.AutoFitRow(0, 1, 0, 1);
                
                Console.WriteLine("AutoFitRow method executed successfully with parameters (0, 1, 0, 1)");
                
                // Visa effekten genom att visa radhöjder
                Console.WriteLine($"Row 1 height after autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height after autofit: {worksheet.Cells.Rows[1].Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitRow method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("AutoFitRowWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int) {#autofitrow}

Anpassar automatiskt radhöjden.

```csharp
public void AutoFitRow(int rowIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindex. |

### Anmärkningar

AutoFitRow är en imprecis funktion.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange lång text med radbrytning i cell A1
            worksheet.Cells["A1"].Value = "LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT";
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Auto-anpassa den första raden
            worksheet.AutoFitRow(0);

            // Spara arbetsboken
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int) {#autofitrow_1}

Anpassar automatiskt radhöjden.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindex. |
| firstColumn | Int32 | Första kolumnens index. |
| lastColumn | Int32 | Sista kolumnens index. |

### Anmärkningar

Denna metod anpassar automatiskt en rad baserat på innehållet i ett cellintervall inom raden.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler som kommer att påverka radens höjd.
            worksheet.Cells["A2"].PutValue("This is a long text that will demonstrate AutoFitRow functionality");
            worksheet.Cells["B2"].PutValue("Additional text in another column");
            
            // Auto-anpassa raden (rad 2) mellan kolumnerna 0 och 1 (A till B).
            worksheet.AutoFitRow(1, 0, 1);
            
            // Spara arbetsboken
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int, AutoFitterOptions) {#autofitrow_2}

Anpassar automatiskt radhöjden.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindex. |
| firstColumn | Int32 | Första kolumnens index. |
| lastColumn | Int32 | Sista kolumnens index. |
| alternativ | AutoFitterOptions | Alternativen för auto-fitter. |

### Anmärkningar

Denna metod anpassar automatiskt en rad baserat på innehållet i ett cellintervall inom raden.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32AutoFitterOptioDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["B1"].PutValue("Another test string in column B");
            
            // Skapa AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                AutoFitMergedCells = true,
                IgnoreHidden = false,
                OnlyAuto = false
            };

            // Hämta den ursprungliga radens höjd.
            double originalHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"Original row height: {originalHeight}");

            // Auto-anpassa den första raden
            worksheet.AutoFitRow(0, 0, 2, options);

            // Hämta den nya radens höjd.
            double newHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"New row height after AutoFit: {newHeight}");

            // Spara arbetsboken
            workbook.Save("AutoFitRowExample.xlsx");
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


