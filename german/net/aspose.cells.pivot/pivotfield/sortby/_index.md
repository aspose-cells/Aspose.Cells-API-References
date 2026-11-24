---
title: "PivotField.SortBy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Sortiert dieses Pivot-Feld"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder) {#sortby}

Sortiert dieses Pivotfeld.

```csharp
public void SortBy(SortOrder sortType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sortType | SortOrder | Der Typ der Sortierung dieses Feldes. |

### Siehe auch

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int) {#sortby_1}

Sortiert dieses Pivotfeld.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method or PivotField.IsAutoSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sortType | SortOrder | Der Typ der Sortierung dieses Feldes. |
| fieldSortedBy | Int32 | Der Index des Pivot-Feldes, nach dem sortiert wird. -1 bedeutet Sortierung nach Datenbeschriftungen dieses Feldes, andere Werte bedeuten den Index des Datenfeldes, nach dem sortiert wird. |

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.SortBy(SortOrder, int,string) oder die Eigenschaft PivotField.IsAutoSort. Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("UK");
            worksheet.Cells["A4"].PutValue("Germany");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Sortieren Sie das Zeilenfeld absteigend mit dem Index -1
            rowField.SortBy(SortOrder.Descending, -1);
            
            // Pivot-Tabelle aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_2}

Sortiert dieses Pivotfeld.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sortType | SortOrder | Der Typ der Sortierung dieses Feldes. |
| fieldSortedBy | Int32 | Der Index des Pivot-Feldes, nach dem sortiert wird. -1 bedeutet Sortierung nach Datenbeschriftungen dieses Feldes, andere Werte bedeuten den Index des Datenfeldes, nach dem sortiert wird. |
| dataType | PivotLineType | Der Typ der sortierten Daten. |
| cellName | String | Nach Werten in der Zeile oder Spalte sortieren |

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.SortBy(SortOrder, int,string). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("B");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);
            worksheet.Cells["B4"].PutValue(100);

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Sortieren Sie das Zeilenfeld
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
            
            // Daten berechnen
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, string) {#sortby_3}

Sortiert dieses Pivotfeld.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sortType | SortOrder | Der Typ der Sortierung dieses Feldes. |
| fieldSortedBy | Int32 | Der Index des Pivot-Feldes, nach dem sortiert wird. -1 bedeutet Sortierung nach Datenbeschriftungen dieses Feldes, andere Werte bedeuten den Index des Datenfeldes, nach dem sortiert wird. |
| cellName | String | Sortieren nach Werten in der Zeile oder Spalte. Wenn Null, nach Gesamtsumme des Feldes gruppieren, sonst nach Werten in der ausgewählten Spalte oder Zeile gruppieren. |

### Siehe auch

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


