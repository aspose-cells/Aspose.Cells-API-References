---
title: Add
second_title: Aspose.Cells för .NET API-referens
description: Lägger till en kommentar till samlingen.
type: docs
weight: 20
url: /sv/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

Lägger till en kommentar till samlingen.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Cellradsindex. |
| column | Int32 | Cell kolumn index. |

### Returvärde

[`Comment`](../../comment) objektindex.

### Exempel

```csharp

[C#]
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";
```

### Se även

* class [CommentCollection](../../commentcollection)
* namnutrymme [Aspose.Cells](../../commentcollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Lägger till en kommentar till samlingen.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellnamn. |

### Returvärde

[`Comment`](../../comment) objektindex.

### Exempel

```csharp

[C#]
int commentIndex2 = comments.Add("B2");
Comment comment2 = comments[commentIndex2];
comment2.Note = "Second note.";
comment2.Font.Name = "Times New Roman";
```

### Se även

* class [CommentCollection](../../commentcollection)
* namnutrymme [Aspose.Cells](../../commentcollection)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
