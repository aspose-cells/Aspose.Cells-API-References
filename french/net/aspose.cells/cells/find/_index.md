---
title: Find
second_title: Référence de l'API Aspose.Cells pour .NET
description: Trouve la cellule contenant lobjet dentrée.
type: docs
weight: 640
url: /fr/net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Trouve la cellule contenant l'objet d'entrée.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| what | Object | L'objet à rechercher. Le type doit être int,double,DateTime,string,bool. |
| previousCell | Cell | Cellule précédente avec le même objet. Ce paramètre peut être défini sur null si la recherche s'effectue depuis le début. |

### Return_Value

Objet cellule.

### Remarques

Renvoie null (Nothing) si aucune cellule n'est trouvée.

### Voir également

* class [Cell](../../cell)
* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Trouve la cellule contenant l'objet d'entrée.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| what | Object | L'objet à rechercher. Le type doit être int,double,DateTime,string,bool. |
| previousCell | Cell | Cellule précédente avec le même objet. Ce paramètre peut être défini sur null si la recherche s'effectue depuis le début. |
| findOptions | FindOptions | Trouver des options |

### Return_Value

Objet cellule.

### Remarques

Renvoie null (Nothing) si aucune cellule n'est trouvée.

### Voir également

* class [Cell](../../cell)
* class [FindOptions](../../findoptions)
* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
