---
title: "Worksheet.AutoFitColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Anpassar automatiskt alla kolumner i detta worksheet"
type: docs
url: /sv/net/aspose.cells/worksheet/autofitcolumns/
---
## AutoFitColumns() {#autofitcolumns}

Anpassar automatiskt alla kolumner i detta kalkylblad.

```csharp
public void AutoFitColumns()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("This is a test string");
            worksheet.Cells["B1"].PutValue("Another longer test string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            
            // Anpassa automatiskt alla kolumner i worksheet
            worksheet.AutoFitColumns();
            
            // Spara arbetsboken
            workbook.Save("AutoFitColumnsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(AutoFitterOptions) {#autofitcolumns_1}

Anpassar automatiskt alla kolumner i detta kalkylblad.

```csharp
public void AutoFitColumns(AutoFitterOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | AutoFitterOptions | Alternativen för automatisk anpassning |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Sample Text for AutoFit");
            worksheet.Cells["B1"].PutValue("Longer Sample Text for Testing AutoFitColumns");
            worksheet.Cells["C1"].PutValue(12345.6789);
            
            // Skapa auto-fitter-alternativ
            AutoFitterOptions options = new AutoFitterOptions();
            options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            
            // Anpassa kolumner automatiskt med alternativ
            worksheet.AutoFitColumns(options);
            
            // Spara arbetsboken
            workbook.Save("AutoFitColumnsWithOptions.xlsx");
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int) {#autofitcolumns_2}

Anpassar automatiskt kolumnbredden.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstColumn | Int32 | Första kolumnens index. |
| lastColumn | Int32 | Sista kolumnens index. |

### Anmärkningar

AutoFitColumn är en inexakt funktion.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att demonstrera autofit
            sheet.Cells["A1"].PutValue("Short");
            sheet.Cells["B1"].PutValue("Medium length text");
            sheet.Cells["C1"].PutValue("Very very long text that needs column width adjustment");
            sheet.Cells["D1"].PutValue("Another example with different length");

            // AutoFit kolumner från index 0 till 3
            sheet.AutoFitColumns(0, 3);

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

---

## AutoFitColumns(int, int, AutoFitterOptions) {#autofitcolumns_3}

Anpassar automatiskt kolumnbredden.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstColumn | Int32 | Första kolumnens index. |
| lastColumn | Int32 | Sista kolumnens index. |
| alternativ | AutoFitterOptions | Alternativen för automatisk anpassning |

### Anmärkningar

AutoFitColumn är en inexakt funktion.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["B1"].PutValue("This is a much longer text that needs column autofitting");
            worksheet.Cells["C1"].PutValue("Another example with different length");

            // Skapa AutoFitterOptions med specifika inställningar
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Anropa AutoFitColumns med parametrarna (firstColumn, lastColumn, options)
                worksheet.AutoFitColumns(0, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, AutoFitterOptions)");
                
                // Visa effekten genom att visa kolumnbredder
                Console.WriteLine($"Column A width: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int) {#autofitcolumns_4}

Anpassar automatiskt kolumnbredden.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Första radens index. |
| firstColumn | Int32 | Första kolumnens index. |
| lastRow | Int32 | Sista radens index. |
| lastColumn | Int32 | Sista kolumnens index. |

### Anmärkningar

AutoFitColumn är en inexakt funktion.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite data för demonstration
            worksheet.Cells["A1"].PutValue("Short");
            worksheet.Cells["B1"].PutValue("Medium length text");
            worksheet.Cells["C1"].PutValue("Very very long text that needs more column width");
            
            // AutoFit kolumner från kolumn 0 (A) till kolumn 2 (C), med första raden 0 och sista raden 0
            worksheet.AutoFitColumns(0, 2, 0, 0);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int, AutoFitterOptions) {#autofitcolumns_5}

Anpassar automatiskt kolumnbredden.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, 
    AutoFitterOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Första radens index. |
| firstColumn | Int32 | Första kolumnens index. |
| lastRow | Int32 | Sista radens index. |
| lastColumn | Int32 | Sista kolumnens index. |
| alternativ | AutoFitterOptions | Alternativen för automatisk anpassning |

### Anmärkningar

AutoFitColumn är en inexakt funktion.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32AutoFitterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll celler med exempeldata som kräver justering av kolumnbredd
            worksheet.Cells["A1"].PutValue("This is a long text that needs column autofit");
            worksheet.Cells["B1"].PutValue("Another lengthy text string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            worksheet.Cells["A2"].PutValue(12345.6789);
            worksheet.Cells["B2"].PutValue("Multi-line\ntext\nsample");
            worksheet.Cells["C2"].PutValue(true);

            // Skapa AutoFitterOptions med specifika inställningar
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Anropa AutoFitColumns med specifika parametrar (firstRow, firstColumn, lastRow, lastColumn, options)
                worksheet.AutoFitColumns(0, 0, 1, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, Int32, Int32, AutoFitterOptions)");
                
                // Visa kolumnbredder efter autofit
                Console.WriteLine($"Column A width after autofit: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width after autofit: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width after autofit: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


