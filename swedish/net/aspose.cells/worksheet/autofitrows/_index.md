---
title: "Worksheet.AutoFitRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Anpassar automatiskt alla rader i detta kalkylblad."
type: docs
url: /sv/net/aspose.cells/worksheet/autofitrows/
---
## AutoFitRows(AutoFitterOptions) {#autofitrows_1}

Anpassar automatiskt alla rader i detta kalkylblad.

```csharp
public void AutoFitRows(AutoFitterOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | AutoFitterOptions | Alternativen för auto-fitter. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempeldata och formatering.
            worksheet.Cells["A1"].PutValue("This is a long text that will need auto-fitting");
            worksheet.Cells["A2"].PutValue("Another long text\nwith multiple lines\nfor demonstration");
            
            // Sammanfoga celler för att demonstrera automatisk anpassning av sammanslagna celler.
            worksheet.Cells.Merge(3, 0, 2, 1);
            worksheet.Cells["A3"].PutValue("Merged cells text that needs to fit");

            // Auto-anpassa rader med specifika alternativ.
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = 100,  // Set reasonable max height
                OnlyAuto = true
            });

            // Spara arbetsboken
            workbook.Save("AutoFitRowsDemo.xlsx");
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

## AutoFitRows(int, int) {#autofitrows_3}

Anpassar automatiskt radhöjden i ett område.

```csharp
public void AutoFitRows(int startRow, int endRow)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradindex. |
| endRow | Int32 | Slutradindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll celler med exempeldata och stilar.
            for (int i = 0; i <= 8; i++)
            {
                Cell cell = cells[i, i];
                cell.Value = "Sample text for row " + i;
                
                if (i % 2 == 0)
                {
                    Style style = cell.GetStyle();
                    style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);
                    cell.SetStyle(style);
                }
            }

            // Auto-anpassa rader från index 0 till 8.
            sheet.AutoFitRows(0, 8);

            // Skriv ut de resulterande radhöjderna.
            for (int i = 0; i <= 8; i++)
            {
                Console.WriteLine($"Row {i} height: {cells.GetRowHeightPixel(i)} pixels");
            }
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}

Anpassar automatiskt radhöjden i ett område.

```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradindex. |
| endRow | Int32 | Slutradindex. |
| alternativ | AutoFitterOptions | Alternativen för auto-fitter. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("This is a test string for auto-fit row height demonstration");
            worksheet.Cells["A2"].PutValue("Another line\nwith multiple lines\nof text");
            
            // Skapa auto-fitter-alternativ
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            
            // Autoanpassa rader 0 till 1 med alternativ
            worksheet.AutoFitRows(0, 1, options);
            
            // Spara arbetsboken
            workbook.Save("AutoFitRowsDemo.xlsx");
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

## AutoFitRows() {#autofitrows}

Anpassar automatiskt alla rader i detta kalkylblad.

```csharp
public void AutoFitRows()
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("This is a test string for AutoFitRows demonstration");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line break to show row height adjustment");
            worksheet.Cells["B1"].PutValue("Column B content");
            
            // Autoanpassa raderna
            worksheet.AutoFitRows();
            
            // Autoanpassa kolumnerna för bättre synlighet
            worksheet.AutoFitColumns();
            
            // Spara arbetsboken
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "AutoFitRowsDemo.xlsx");
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Worksheet with AutoFitRows saved to: " + outputPath);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(bool) {#autofitrows_2}

Anpassar automatiskt alla rader i detta kalkylblad.

```csharp
public void AutoFitRows(bool onlyAuto)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| onlyAuto | Boolean | Sant, autoanpassar endast radhöjden när radhöjden inte är anpassad. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeltext i celler för att demonstrera radautoanpassning
            worksheet.Cells["A1"].PutValue("This is a sample text that will demonstrate AutoFitRows functionality");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line breaks\nto show multi-line row adjustment");
            
            // Autoanpassa rader med hänsyn till automatisk sammanslagning
            worksheet.AutoFitRows(true);
            
            // Spara arbetsboken
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


