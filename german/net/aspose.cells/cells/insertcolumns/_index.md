---
title: "Cells.InsertColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Fügt einige Spalten in das Arbeitsblatt ein"
type: docs
url: /de/net/aspose.cells/cells/insertcolumns/
---
## InsertColumns(int, int) {#insertcolumns}

Fügt mehrere Spalten in das Arbeitsblatt ein.

```csharp
public void InsertColumns(int columnIndex, int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex. |
| totalColumns | Int32 | Die Anzahl der Spalten. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie 3 Spalten ein, beginnend bei Spaltenindex 1 (zweite Spalte)
            worksheet.Cells.InsertColumns(1, 3);
            
            // Fügen Sie Beispieldaten hinzu, um die eingefügten Spalten zu demonstrieren
            worksheet.Cells["A1"].PutValue("Original Column");
            worksheet.Cells["B1"].PutValue("Inserted Column 1");
            worksheet.Cells["C1"].PutValue("Inserted Column 2");
            worksheet.Cells["D1"].PutValue("Inserted Column 3");
            worksheet.Cells["E1"].PutValue("Original Column 2");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, bool) {#insertcolumns_2}

Fügt mehrere Spalten in das Arbeitsblatt ein.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex. |
| totalColumns | Int32 | Die Anzahl der Spalten. |
| updateReference | Boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie 3 Spalten bei Spaltenindex 2 (0-basiert) ein und verschieben die vorhandenen Spalten nach rechts
            worksheet.Cells.InsertColumns(2, 3, true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, InsertOptions) {#insertcolumns_1}

Fügt mehrere Spalten in das Arbeitsblatt ein.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, InsertOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex. |
| totalColumns | Int32 | Die Anzahl der Spalten. |
| Optionen | InsertOptions | Die Optionen für den Einfügevorgang. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // Einfügeoptionen erstellen
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.Clear;

            // Fügen Sie eine Spalte bei Index 1 (zweite Spalte) ein
            worksheet.Cells.InsertColumns(1, 1, options);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


