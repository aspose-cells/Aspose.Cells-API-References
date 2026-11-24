---
title: "GridNameCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridNameCollection-Methode. Definiert einen neuen globalen Namen"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridnamecollection/add/
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
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, string, string) {#add}

Definiert einen neuen Namen im angegebenen Blatt.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| Parameter | Beschreibung |
| --- | --- |
| sheetIndex | Der Blatt-Index, in dem der Name angewendet wird. |
| Text | Namens-Text. Er darf keinen Blattnamen haben. |
| refersTo | Die Formel, auf die der Name verweist. Sie muss einen Blattnamen enthalten, z.B. 'sheet hello!'A1:B2. |
| sheetIndex | Der SheetIndex des Namens, der Index beginnt bei 1. |

### Rückgabewert

Name-Objekt-Index.

### Siehe auch

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


