---
title: "GridNameCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridNameCollection-Methode. Definiert einen neuen globalen Namen"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridnamecollection/add/
---
## Add(string, string) {#add_1}

Definiert einen neuen globalen Namen.

```csharp
public int Add(string text, string refersTo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Namens-Text. Er kann einen Blattnamen haben. |
| refersTo | String | Die Formel, auf die der Name verweist. Sie muss einen Blattnamen enthalten, z.B. 'sheet hello!'A1:B2. |

### Rückgabewert

Name-Objekt-Index.

### Siehe auch

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(int, string, string) {#add}

Definiert einen neuen Namen im angegebenen Blatt.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | Int32 | Der Blatt-Index, in dem der Name angewendet wird. |
| Text | String | Namens-Text. Er darf keinen Blattnamen haben. |
| refersTo | String | Die Formel, auf die der Name verweist. Sie muss einen Blattnamen enthalten, z.B. 'sheet hello!'A1:B2. |

### Rückgabewert

Name-Objekt-Index.

### Siehe auch

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


