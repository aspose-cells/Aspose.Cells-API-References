---
title: "GridWorksheet.FreezePanes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridWorksheet-Methode. Friert die Bereiche an der angegebenen Zelle im Arbeitsblatt ein."
type: docs
url: /de/net/aspose.cells.gridweb.data/gridworksheet/freezepanes/
---
## FreezePanes(string, int, int) {#freezepanes_1}

Friert die Bildschirmelemente an der angegebenen Zelle im Arbeitsblatt ein.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Zellname. |
| freezedRows | Int32 | Anzahl der sichtbaren Zeilen im oberen Bereich, nicht mehr als Zeilenindex. |
| freezedColumns | Int32 | Anzahl der sichtbaren Spalten im linken Bereich, nicht mehr als Spaltenindex. |

### Hinweise

Zeilenindex und Spaltenindex können nicht alle Null sein. Die Anzahl der Zeilen und die Anzahl der Spalten können ebenfalls nicht alle Null sein.

### Siehe auch

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## FreezePanes(int, int, int, int) {#freezepanes}

Friert die Bildschirmelemente an der angegebenen Zelle im Arbeitsblatt ein.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |
| column | Int32 | Spaltenindex. |
| freezedRows | Int32 | Anzahl der sichtbaren Zeilen im oberen Bereich, nicht mehr als Zeilenindex. |
| freezedColumns | Int32 | Anzahl der sichtbaren Spalten im linken Bereich, nicht mehr als Spaltenindex. |

### Hinweise

Zeilenindex und Spaltenindex können nicht alle Null sein. Die Anzahl der Zeilen und die Anzahl der Spalten können ebenfalls nicht alle Null sein.

Die ersten beiden Parameter geben die eingefrorene Position an und die letzten beiden Parameter geben den im linken oberen Bereich eingefrorenen Bereich an.

### Siehe auch

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


