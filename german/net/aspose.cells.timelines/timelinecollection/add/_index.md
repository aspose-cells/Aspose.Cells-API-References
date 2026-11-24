---
title: "TimelineCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TimelineCollection-Methode. Fügt ein neues Timeline hinzu, das PivotTable als Datenquelle verwendet."
type: docs
url: /de/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Füge eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Timeline‑Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Timeline‑Bereichs. |
| baseFieldName | String | Der Name des PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Timeline-Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 1, 3);
            cells["C4"].Value = 200;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Column, 1);
            pivot.AddFieldToArea(PivotFieldType.Data, 2);

            // Timeline hinzufügen, die mit der Pivot-Tabelle verbunden ist.
            sheet.Timelines.Add(pivot, 10, 5, "Date");
            
            // Arbeitsmappe speichern.
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Füge eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Der Zellname in der oberen linken Ecke des Timeline‑Bereichs. |
| baseFieldName | String | Der Name des PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Timeline-Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            
            // PivotTable hinzufügen
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "C1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Timeline hinzufügen, die mit der Pivot-Tabelle verbunden ist.
            sheet.Timelines.Add(pivot, "E1", "Date");
            
            // Speichere die Arbeitsmappe
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Füge eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Timeline‑Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Timeline‑Bereichs. |
| baseFieldIndex | Int32 | Der Index des PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Timeline-Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // PivotTable hinzufügen
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Timeline-Steuerelement hinzufügen.
            sheet.Timelines.Add(pivot, 15, 5, 1);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Füge eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Der Zellname in der oberen linken Ecke des Timeline‑Bereichs. |
| baseFieldIndex | Int32 | Der Index des PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Timeline-Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Date");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue(new DateTime(2023, 1, 1));
            cells["B2"].PutValue("A");
            cells["C2"].PutValue(100);
            
            cells["A3"].PutValue(new DateTime(2023, 1, 2));
            cells["B3"].PutValue("B");
            cells["C3"].PutValue(200);
            
            cells["A4"].PutValue(new DateTime(2023, 1, 3));
            cells["B4"].PutValue("A");
            cells["C4"].PutValue(150);

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot-Tabellendaten aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Basisfeld-Index für das Feld "Date" finden.
            int dateFieldIndex = -1;
            for (int i = 0; i < pivotTable.BaseFields.Count; i++)
            {
                if (pivotTable.BaseFields[i].Name == "Date")
                {
                    dateFieldIndex = i;
                    break;
                }
            }

            // Timeline hinzufügen mit dem gefundenen Index.
            if (dateFieldIndex >= 0)
            {
                sheet.Timelines.Add(pivotTable, "H2", dateFieldIndex);
            }

            // Ergebnis speichern
            workbook.Save("TimelineCollectionMethodAddWithPivotTableStringInt32Demo_output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Füge eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Timeline‑Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Timeline‑Bereichs. |
| baseField | PivotField | Das PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Timeline-Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 2, 1);
            cells["C4"].Value = 200;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            
            // Pivot-Felder hinzufügen.
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);
            pivot.AddFieldToArea(PivotFieldType.Column, pivot.BaseFields[1]);
            pivot.AddFieldToArea(PivotFieldType.Data, pivot.BaseFields[2]);

            // Zeitachse mit der Pivot-Tabelle hinzufügen
            sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
            
            // Speichere die Arbeitsmappe
            workbook.Save("TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Füge eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Der Zellname in der oberen linken Ecke des Timeline‑Bereichs. |
| baseField | PivotField | Das PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Timeline-Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivot.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Zeitachse hinzufügen, indem die Pivot-Tabelle als Datenquelle verwendet wird
            sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[0]);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


