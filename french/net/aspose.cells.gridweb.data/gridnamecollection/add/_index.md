---
title: "GridNameCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridNameCollection méthode. Définit un nouveau nom global"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridnamecollection/add/
---
## Add(string, string) {#add_1}

Définit un nouveau nom global.

```csharp
public int Add(string text, string refersTo)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | Texte du nom. Il peut contenir le nom de la feuille. |
| refersTo | String | La formule à laquelle le nom fait référence. Elle doit contenir le nom de la feuille, par ex. 'sheet hello!'A1:B2. |

### Valeur de retour

Index de l'objet Name.

### Voir aussi

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(int, string, string) {#add}

Définit un nouveau nom dans la feuille spécifiée.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | L'index de la feuille dans lequel le nom est appliqué. |
| texte | String | Texte du nom. Il ne peut pas contenir le nom de la feuille. |
| refersTo | String | La formule à laquelle le nom fait référence. Elle doit contenir le nom de la feuille, par ex. 'sheet hello!'A1:B2. |

### Valeur de retour

Index de l'objet Name.

### Voir aussi

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


