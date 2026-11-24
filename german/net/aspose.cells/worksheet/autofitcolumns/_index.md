---
title: "Worksheet.AutoFitColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Passt automatisch alle Spalten in diesem Arbeitsblatt an"
type: docs
url: /de/net/aspose.cells/worksheet/autofitcolumns/
---
## AutoFitColumns() {#autofitcolumns}

Passt alle Spalten in diesem Arbeitsblatt automatisch an.

```csharp
public void AutoFitColumns()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("This is a test string");
            worksheet.Cells["B1"].PutValue("Another longer test string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            
            // Alle Spalten im Arbeitsblatt automatisch anpassen
            worksheet.AutoFitColumns();
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitColumnsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(AutoFitterOptions) {#autofitcolumns_1}

Passt alle Spalten in diesem Arbeitsblatt automatisch an.

```csharp
public void AutoFitColumns(AutoFitterOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | AutoFitterOptions | Die Optionen für das automatische Anpassen |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Sample Text for AutoFit");
            worksheet.Cells["B1"].PutValue("Longer Sample Text for Testing AutoFitColumns");
            worksheet.Cells["C1"].PutValue(12345.6789);
            
            // AutoFitter-Optionen erstellen
            AutoFitterOptions options = new AutoFitterOptions();
            options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            
            // Spalten mit Optionen automatisch anpassen
            worksheet.AutoFitColumns(options);
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitColumnsWithOptions.xlsx");
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

## AutoFitColumns(int, int) {#autofitcolumns_2}

Passt die Spaltenbreite automatisch an.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstColumn | Int32 | Erster Spaltenindex. |
| lastColumn | Int32 | Letzter Spaltenindex. |

### Hinweise

AutoFitColumn ist eine ungenaue Funktion.

### Beispiele

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

            // Beispieldaten hinzufügen, um das automatische Anpassen zu demonstrieren
            sheet.Cells["A1"].PutValue("Short");
            sheet.Cells["B1"].PutValue("Medium length text");
            sheet.Cells["C1"].PutValue("Very very long text that needs column width adjustment");
            sheet.Cells["D1"].PutValue("Another example with different length");

            // AutoFit-Spalten von Index 0 bis 3
            sheet.AutoFitColumns(0, 3);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, AutoFitterOptions) {#autofitcolumns_3}

Passt die Spaltenbreite automatisch an.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstColumn | Int32 | Erster Spaltenindex. |
| lastColumn | Int32 | Letzter Spaltenindex. |
| Optionen | AutoFitterOptions | Die Optionen für das automatische Anpassen |

### Hinweise

AutoFitColumn ist eine ungenaue Funktion.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["B1"].PutValue("This is a much longer text that needs column autofitting");
            worksheet.Cells["C1"].PutValue("Another example with different length");

            // AutoFitterOptions mit spezifischen Einstellungen erstellen
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Rufen Sie AutoFitColumns mit den Parametern (firstColumn, lastColumn, options) auf
                worksheet.AutoFitColumns(0, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, AutoFitterOptions)");
                
                // Zeigen Sie die Wirkung, indem Sie die Spaltenbreiten anzeigen
                Console.WriteLine($"Column A width: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
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

## AutoFitColumns(int, int, int, int) {#autofitcolumns_4}

Passt die Spaltenbreite automatisch an.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Index der ersten Zeile. |
| firstColumn | Int32 | Erster Spaltenindex. |
| lastRow | Int32 | Index der letzten Zeile. |
| lastColumn | Int32 | Letzter Spaltenindex. |

### Hinweise

AutoFitColumn ist eine ungenaue Funktion.

### Beispiele

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
            
            // Füllen Sie einige Daten zur Demonstration ein
            worksheet.Cells["A1"].PutValue("Short");
            worksheet.Cells["B1"].PutValue("Medium length text");
            worksheet.Cells["C1"].PutValue("Very very long text that needs more column width");
            
            // AutoFit-Spalten von Spalte 0 (A) bis Spalte 2 (C), mit erster Zeile 0 und letzter Zeile 0
            worksheet.AutoFitColumns(0, 2, 0, 0);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int, AutoFitterOptions) {#autofitcolumns_5}

Passt die Spaltenbreite automatisch an.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, 
    AutoFitterOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Index der ersten Zeile. |
| firstColumn | Int32 | Erster Spaltenindex. |
| lastRow | Int32 | Index der letzten Zeile. |
| lastColumn | Int32 | Letzter Spaltenindex. |
| Optionen | AutoFitterOptions | Die Optionen für das automatische Anpassen |

### Hinweise

AutoFitColumn ist eine ungenaue Funktion.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32AutoFitterDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füllen Sie Zellen mit Beispieldaten, die eine Anpassung der Spaltenbreite benötigen
            worksheet.Cells["A1"].PutValue("This is a long text that needs column autofit");
            worksheet.Cells["B1"].PutValue("Another lengthy text string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            worksheet.Cells["A2"].PutValue(12345.6789);
            worksheet.Cells["B2"].PutValue("Multi-line\ntext\nsample");
            worksheet.Cells["C2"].PutValue(true);

            // AutoFitterOptions mit spezifischen Einstellungen erstellen
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Rufen Sie AutoFitColumns mit spezifischen Parametern (firstRow, firstColumn, lastRow, lastColumn, options) auf
                worksheet.AutoFitColumns(0, 0, 1, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, Int32, Int32, AutoFitterOptions)");
                
                // Zeigen Sie die Spaltenbreiten nach dem AutoFit an
                Console.WriteLine($"Column A width after autofit: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width after autofit: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width after autofit: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


