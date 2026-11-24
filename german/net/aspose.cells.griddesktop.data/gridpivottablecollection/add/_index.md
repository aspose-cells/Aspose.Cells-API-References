---
title: "GridPivotTableCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridPivotTableCollection-Methode. Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridpivottablecollection/add/
---
## Add(string, string, string) {#add_3}

Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Zellbereich der Daten für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| destCellName | String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Siehe auch

* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(Worksheet, GridCellArea, string, string) {#add}

Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu.

```csharp
public int Add(Worksheet sourceSheet, GridCellArea sourceArea, string destCellName, 
    string tableName)
```

| Parameter | Beschreibung |
| --- | --- |
| sourceSheet | Das Quell-Arbeitsblatt. |
| sourceArea | Der Bereich im Quell-Arbeitsblatt. |
| destRow | Die Zeile der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| destCol | Die Spalte der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Siehe auch

* class [Worksheet](../../../aspose.cells.griddesktop/worksheet/)
* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, int, int, string) {#add_1}

Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, int destRow, int destCol, 
    string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| worksheetname | String | Der Name des Quell-Arbeitsblatts. |
| sourceArea | GridCellArea | Der Bereich im Quell-Arbeitsblatt. |
| destRow | Int32 | Die Zeile der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| destCol | Int32 | Die Spalte der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Siehe auch

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, string, string) {#add_2}

Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, string destCellName, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| worksheetname | String | Der Name des Quell-Arbeitsblatts. |
| sourceArea | GridCellArea | Der Bereich im Quell-Arbeitsblatt. |
| destCellName | String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Siehe auch

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


