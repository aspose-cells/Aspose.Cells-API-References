---
title: "GridCells.DeleteRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCells-Methode. Löscht mehrere Zeilen"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridcells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Löscht mehrere Zeilen.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Der Index der ersten zu löschenden Zeile. |
| totalRows | Int32 | Anzahl der zu löschenden Zeilen. |

### Hinweise

Wenn der gelöschte Bereich den oberen Teil (nicht das Ganze) der Tabelle (ListObject) enthält, kann der Bereich nicht gelöscht werden und es wird nichts unternommen. Es funktioniert wie in MS Excel.

### Siehe auch

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

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

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


