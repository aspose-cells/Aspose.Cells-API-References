---
title: Add
second_title: Aspose.Cells für .NET-API-Referenz
description: Definiert einen neuen globalen Namen.
type: docs
weight: 30
url: /de/net/aspose.cells.gridweb.data/gridnamecollection/add/
---
## Add(string, string) {#add_1}

Definiert einen neuen globalen Namen.

```csharp
public int Add(string text, string refersTo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| text | String | Name text.It kann Blattname haben. |
| refersTo | String | Die Formel, auf die sich der Name beziehen soll. Sie muss einen Blattnamen haben, z. B. „Blatt Hallo!“ A1:B2. |

### Rückgabewert

Objektindex benennen.

### Siehe auch

* class [GridNameCollection](../../gridnamecollection)
* namensraum [Aspose.Cells.GridWeb.Data](../../gridnamecollection)
* Montage [Aspose.Cells.GridWeb](../../../)

---

## Add(int, string, string) {#add}

Definiert einen neuen Namen im angegebenen Blatt.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| Parameter | Beschreibung |
| --- | --- |
| sheetIndex | Der Blattindex, in dem der Name angewendet wird. |
| text | Namenstext. Er darf keinen Blattnamen haben. |
| refersTo | Die Formel, auf die sich der Name beziehen soll. Sie muss Blattname haben, z. B. 'Blatt Hallo!'A1:B2. |
| sheetIndex | SheetIndex des Namens, der Index ist von 1. |

### Rückgabewert

Objektindex benennen.

### Siehe auch

* class [GridNameCollection](../../gridnamecollection)
* namensraum [Aspose.Cells.GridWeb.Data](../../gridnamecollection)
* Montage [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->