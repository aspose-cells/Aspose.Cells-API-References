---
title: "Worksheet.AutoFitRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Passt die Zeilenhöhe in einem rechteckigen Bereich automatisch an"
type: docs
url: /de/net/aspose.cells/worksheet/autofitrow/
---
## AutoFitRow(int, int, int, int) {#autofitrow_3}

Passt die Zeilenhöhe in einem rechteckigen Bereich automatisch an.

```csharp
public void AutoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Startzeilenindex. |
| endRow | Int32 | Endzeilenindex. |
| startColumn | Int32 | Startspaltenindex. |
| endColumn | Int32 | Endspaltenindex. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            RowCollection rows = worksheet.Cells.Rows;
            rows[0].Height = 20;
            rows[1].Height = 20;
            // Beispieldaten zu Zellen hinzufügen, um die automatische Zeilenanpassung zu demonstrieren
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row autofit");
            worksheet.Cells["B1"].PutValue("Additional column with text");
            worksheet.Cells["A2"].PutValue("Shorter text");
            worksheet.Cells["B2"].PutValue("More text");
            
            try
            {
                Console.WriteLine($"Row 1 height before autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height before autofit: {worksheet.Cells.Rows[1].Height}");

                // Rufen Sie AutoFitRow mit den Parametern auf: startRow, endRow, startColumn, endColumn
                worksheet.AutoFitRow(0, 1, 0, 1);
                
                Console.WriteLine("AutoFitRow method executed successfully with parameters (0, 1, 0, 1)");
                
                // Zeigen Sie die Wirkung, indem Sie die Zeilenhöhen anzeigen
                Console.WriteLine($"Row 1 height after autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height after autofit: {worksheet.Cells.Rows[1].Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitRow method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("AutoFitRowWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int) {#autofitrow}

Passt die Zeilenhöhe automatisch an.

```csharp
public void AutoFitRow(int rowIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Zeilenindex. |

### Hinweise

AutoFitRow ist eine ungenaue Funktion.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Legen Sie langen Text mit Zeilenumbruch in Zelle A1 fest
            worksheet.Cells["A1"].Value = "LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT";
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Erste Zeile automatisch anpassen
            worksheet.AutoFitRow(0);

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int) {#autofitrow_1}

Passt die Zeilenhöhe automatisch an.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Zeilenindex. |
| firstColumn | Int32 | Erster Spaltenindex. |
| lastColumn | Int32 | Letzter Spaltenindex. |

### Hinweise

Diese Methode passt eine Zeile automatisch an den Inhalt eines Zellbereichs innerhalb der Zeile an.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zu Zellen hinzufügen, die die Zeilenhöhe beeinflussen
            worksheet.Cells["A2"].PutValue("This is a long text that will demonstrate AutoFitRow functionality");
            worksheet.Cells["B2"].PutValue("Additional text in another column");
            
            // AutoFit die Zeile (Zeile 2) zwischen den Spalten 0 und 1 (A bis B)
            worksheet.AutoFitRow(1, 0, 1);
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int, AutoFitterOptions) {#autofitrow_2}

Passt die Zeilenhöhe automatisch an.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Zeilenindex. |
| firstColumn | Int32 | Erster Spaltenindex. |
| lastColumn | Int32 | Letzter Spaltenindex. |
| Optionen | AutoFitterOptions | Die AutoFitter-Optionen |

### Hinweise

Diese Methode passt eine Zeile automatisch an den Inhalt eines Zellbereichs innerhalb der Zeile an.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32AutoFitterOptioDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["B1"].PutValue("Another test string in column B");
            
            // AutoFitterOptions erstellen
            AutoFitterOptions options = new AutoFitterOptions
            {
                AutoFitMergedCells = true,
                IgnoreHidden = false,
                OnlyAuto = false
            };

            // Ursprüngliche Zeilenhöhe abrufen
            double originalHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"Original row height: {originalHeight}");

            // AutoFit die erste Zeile
            worksheet.AutoFitRow(0, 0, 2, options);

            // Neue Zeilenhöhe abrufen
            double newHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"New row height after AutoFit: {newHeight}");

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitRowExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


