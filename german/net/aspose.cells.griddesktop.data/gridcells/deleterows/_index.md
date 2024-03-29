---
title: DeleteRows
second_title: Aspose.Cells für .NET-API-Referenz
description: Löscht mehrere Zeilen.
type: docs
weight: 360
url: /de/net/aspose.cells.griddesktop.data/gridcells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Löscht mehrere Zeilen.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Der erste zu löschende Zeilenindex. |
| totalRows | Int32 | Anzahl der zu löschenden Zeilen. |

### Bemerkungen

Wenn der gelöschte Bereich den oberen Teil (nicht ganz) der Tabelle (ListObject) enthält, konnte der Bereich nicht gelöscht werden und es wird nichts getan. Es funktioniert wie MS Excel.

### Siehe auch

* class [GridCells](../../gridcells)
* namensraum [Aspose.Cells.GridDesktop.Data](../../gridcells)
* Montage [Aspose.Cells.GridDesktop](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_1}

Löscht mehrere Zeilen im Arbeitsblatt.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Zeilenindex. |
| totalRows | Int32 | Anzahl der zu löschenden Zeilen. |
| updateReference | Boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### Siehe auch

* class [GridCells](../../gridcells)
* namensraum [Aspose.Cells.GridDesktop.Data](../../gridcells)
* Montage [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
