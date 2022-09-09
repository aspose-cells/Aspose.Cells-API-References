---
title: Add
second_title: Aspose.Cells für .NET-API-Referenz
description: Fügt der Sammlung einen Kommentar hinzu.
type: docs
weight: 20
url: /de/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

Fügt der Sammlung einen Kommentar hinzu.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zellenzeilenindex. |
| column | Int32 | Zellspaltenindex. |

### Rückgabewert

[`Comment`](../../comment) Objektindex.

### Beispiele

```csharp

[C#]
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";
```

### Siehe auch

* class [CommentCollection](../../commentcollection)
* namensraum [Aspose.Cells](../../commentcollection)
* Montage [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Fügt der Sammlung einen Kommentar hinzu.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Zellenname. |

### Rückgabewert

[`Comment`](../../comment) Objektindex.

### Beispiele

```csharp

[C#]
int commentIndex2 = comments.Add("B2");
Comment comment2 = comments[commentIndex2];
comment2.Note = "Second note.";
comment2.Font.Name = "Times New Roman";
```

### Siehe auch

* class [CommentCollection](../../commentcollection)
* namensraum [Aspose.Cells](../../commentcollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->