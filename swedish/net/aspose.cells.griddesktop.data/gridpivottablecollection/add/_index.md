---
title: "GridPivotTableCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridPivotTableCollection-metod. Lägger till en ny PivotTable-cache i en PivotCaches-samling"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridpivottablecollection/add/
---
## Add(string, string, string) {#add_3}

Lägger till en ny PivotTable‑cache i en PivotCaches‑samling.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | String | Datacellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| destCellName | String | Cellen i det övre vänstra hörnet av PivotTable-rapportens destinationsområde. |
| tableName | String | Namnet på den nya PivotTable-rapporten. |

### Returvärde

Index för den nylagda cachen.

### Se även

* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(Worksheet, GridCellArea, string, string) {#add}

Lägger till en ny PivotTable‑cache i en PivotCaches‑samling.

```csharp
public int Add(Worksheet sourceSheet, GridCellArea sourceArea, string destCellName, 
    string tableName)
```

| Parameter | Beskrivning |
| --- | --- |
| sourceSheet | Källarbetsbladet. |
| sourceArea | Området i källarbetsbladet. |
| destRow | Raden för cellen i det övre vänstra hörnet av PivotTable-rapportens destinationsområde. |
| destCol | Kolumnen för cellen i det övre vänstra hörnet av PivotTable-rapportens destinationsområde. |
| tableName | Namnet på den nya PivotTable-rapporten. |

### Returvärde

Index för den nylagda cachen.

### Se även

* class [Worksheet](../../../aspose.cells.griddesktop/worksheet/)
* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, int, int, string) {#add_1}

Lägger till en ny PivotTable‑cache i en PivotCaches‑samling.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, int destRow, int destCol, 
    string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| worksheetname | String | Namnet på källarbetsbladet. |
| sourceArea | GridCellArea | Området i källarbetsbladet. |
| destRow | Int32 | Raden för cellen i det övre vänstra hörnet av PivotTable-rapportens destinationsområde. |
| destCol | Int32 | Kolumnen för cellen i det övre vänstra hörnet av PivotTable-rapportens destinationsområde. |
| tableName | String | Namnet på den nya PivotTable-rapporten. |

### Returvärde

Index för den nylagda cachen.

### Se även

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, string, string) {#add_2}

Lägger till en ny PivotTable‑cache i en PivotCaches‑samling.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, string destCellName, string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| worksheetname | String | Namnet på källarbetsbladet. |
| sourceArea | GridCellArea | Området i källarbetsbladet. |
| destCellName | String | Cellen i det övre vänstra hörnet av PivotTable-rapportens destinationsområde. |
| tableName | String | Namnet på den nya PivotTable-rapporten. |

### Returvärde

Index för den nylagda cachen.

### Se även

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


