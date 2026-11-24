---
title: "SlicerCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SlicerCollection-Methode. Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet"
type: docs
url: /de/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Fügen Sie einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet.

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseFieldName | String | Der Name des PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Slicer-Index

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];

            // Füge Slicer hinzu
            int slicerIndex = worksheet.Slicers.Add(pivot, "E3", "fruit");
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Fügen Sie einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet.

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseFieldName | String | Der Name des PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Slicer-Index

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Fruit");
            cells["B1"].PutValue("Quantity");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(50);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(30);

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Füge Slicer hinzu
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivotTable, 20, 12, "fruit");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Fügen Sie einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet.

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseFieldIndex | Int32 | Der Index des PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Slicer-Index

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // PivotTable hinzufügen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Slicer für die Pivot-Tabelle hinzufügen
            int slicerIndex = worksheet.Slicers.Add(pivot, 20, 8, 0);
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Fügen Sie einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet.

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseFieldIndex | Int32 | Der Index des PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Slicer-Index

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Füge Slicer hinzu
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "A1", 0);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Fügen Sie einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet.

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseField | PivotField | Das PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Slicer-Index

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 7;

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Pivot-Felder hinzufügen.
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Füge Slicer hinzu
            int slicerIndex = sheet.Slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Speichere die Arbeitsmappe
            workbook.Save("SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Fügen Sie einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet.

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseField | PivotField | Das PivotField in PivotTable.BaseFields. |

### Rückgabewert

Der neue hinzugefügte Slicer-Index

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);

            // Füge Slicer hinzu
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "I3", pivot.BaseFields[0]);

            // Speichere die Arbeitsmappe
            workbook.Save("SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Fügen Sie einen neuen Slicer hinzu, der ListObjet als Datenquelle verwendet.

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Tabelle | ListObject | ListObject-Objekt |
| Index | Int32 | Der Index von ListColumn in ListObject.ListColumns |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |

### Rückgabewert

Der neue hinzugefügte Slicer-Index

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und ListObject erstellen
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue("E38");
            worksheet.Cells["A3"].PutValue("E39");
            worksheet.Cells["A4"].PutValue("E40");
            
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Slicer für das ListObject hinzufügen - Hinweis: Slicers.Add gibt den int-Index zurück
            int slicerIndex = worksheet.Slicers.Add(listObject, 0, "E38");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Speichere die Arbeitsmappe
            workbook.Save("SlicerCollectionMethodAddWithListObjectInt32StringDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Fügen Sie einen neuen Slicer hinzu, der ListObjet als Datenquelle verwendet.

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Tabelle | ListObject | ListObject-Objekt |
| listColumn | ListColumn | Die ListColumn in ListObject.ListColumns |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |

### Rückgabewert

Der neue hinzugefügte Slicer-Index

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");

            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

            SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(table, table.ListColumns[1], "I38");

            worksheet.Cells.SetColumnWidth(0, 20);
            worksheet.Cells.SetColumnWidth(1, 20);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Fügen Sie einen neuen Slicer hinzu, der ListObjet als Datenquelle verwendet.

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Tabelle | ListObject | ListObject-Objekt |
| listColumn | ListColumn | Die ListColumn in ListObject.ListColumns |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |

### Rückgabewert

Der neue hinzugefügte Slicer-Index

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnInt32Int32Demo
    {
        public static void Run()
        {
            // Arbeitsmappe erstellen
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispieldaten für die Tabelle hinzufügen
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue("CatA");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue("CatB");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue("CatA");
            
            // Tabellenbereich erstellen
            int endRow = 4;
            string startCell = "A1";
            string endCell = $"B{endRow}";
            
            // Tabelle zum Arbeitsblatt hinzufügen unter Verwendung der richtigen Überladung
            int tableIndex = sheet.ListObjects.Add(startCell, endCell, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Slicer für die Spalte Category an Position (Zeile 6, Spalte 1) hinzufügen
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(table, table.ListColumns[1], 6, 1);
            
            // Ergebnis speichern
            workbook.Save("SlicerOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


