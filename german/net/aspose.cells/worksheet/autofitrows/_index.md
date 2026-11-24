---
title: "Worksheet.AutoFitRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Passt alle Zeilen in diesem Arbeitsblatt automatisch an"
type: docs
url: /de/net/aspose.cells/worksheet/autofitrows/
---
## AutoFitRows(AutoFitterOptions) {#autofitrows_1}

Passt alle Zeilen in diesem Arbeitsblatt automatisch an.

```csharp
public void AutoFitRows(AutoFitterOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | AutoFitterOptions | Die AutoFitter-Optionen |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten und Formatierung festlegen
            worksheet.Cells["A1"].PutValue("This is a long text that will need auto-fitting");
            worksheet.Cells["A2"].PutValue("Another long text\nwith multiple lines\nfor demonstration");
            
            // Zellen zusammenführen, um das automatische Anpassen zusammengeführter Zellen zu demonstrieren
            worksheet.Cells.Merge(3, 0, 2, 1);
            worksheet.Cells["A3"].PutValue("Merged cells text that needs to fit");

            // AutoFit Zeilen mit spezifischen Optionen
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = 100,  // Set reasonable max height
                OnlyAuto = true
            });

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int) {#autofitrows_3}

Passt die Zeilenhöhe in einem Bereich automatisch an.

```csharp
public void AutoFitRows(int startRow, int endRow)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Startzeilenindex. |
| endRow | Int32 | Endzeilenindex. |

### Beispiele

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

            // Zellen mit Beispieldaten und Stilen füllen
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

            // Auto-fit Zeilen von Index 0 bis 8
            sheet.AutoFitRows(0, 8);

            // Gib die resultierenden Zeilenhöhen aus
            for (int i = 0; i <= 8; i++)
            {
                Console.WriteLine($"Row {i} height: {cells.GetRowHeightPixel(i)} pixels");
            }
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}

Passt die Zeilenhöhe in einem Bereich automatisch an.

```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Startzeilenindex. |
| endRow | Int32 | Endzeilenindex. |
| Optionen | AutoFitterOptions | Die Optionen des AutoFitters. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("This is a test string for auto-fit row height demonstration");
            worksheet.Cells["A2"].PutValue("Another line\nwith multiple lines\nof text");
            
            // AutoFitter-Optionen erstellen
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            
            // Auto fit Zeilen 0 bis 1 mit Optionen
            worksheet.AutoFitRows(0, 1, options);
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows() {#autofitrows}

Passt alle Zeilen in diesem Arbeitsblatt automatisch an.

```csharp
public void AutoFitRows()
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("This is a test string for AutoFitRows demonstration");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line break to show row height adjustment");
            worksheet.Cells["B1"].PutValue("Column B content");
            
            // AutoFit die Zeilen
            worksheet.AutoFitRows();
            
            // AutoFit die Spalten für bessere Sichtbarkeit
            worksheet.AutoFitColumns();
            
            // Speichere die Arbeitsmappe
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "AutoFitRowsDemo.xlsx");
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Worksheet with AutoFitRows saved to: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(bool) {#autofitrows_2}

Passt alle Zeilen in diesem Arbeitsblatt automatisch an.

```csharp
public void AutoFitRows(bool onlyAuto)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| onlyAuto | Boolean | True, passt die Zeilenhöhe nur automatisch an, wenn die Zeilenhöhe nicht benutzerdefiniert ist. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieltext zu Zellen hinzufügen, um die automatische Zeilenanpassung zu demonstrieren
            worksheet.Cells["A1"].PutValue("This is a sample text that will demonstrate AutoFitRows functionality");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line breaks\nto show multi-line row adjustment");
            
            // Zeilen automatisch anpassen unter Berücksichtigung von automatischem Zusammenführen
            worksheet.AutoFitRows(true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


