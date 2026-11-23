---
title: "PivotField.Top10AutoShow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Configure les paramètres Top10 AutoShow pour ce champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

Configure les paramètres Top10 AutoShow pour ce champ pivot.

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isAutoShow | Boolean | true pour activer AutoShow ; false pour désactiver. |
| isTop | Boolean | Si true, affiche les éléments supérieurs ; false affiche les éléments inférieurs. |
| nombre | Int32 | Nombre d'éléments supérieurs/inférieurs à afficher. |
| rankBy | Int32 | Index du champ de données utilisé pour le classement. Utilisez -1 pour classer par les propres valeurs du pivotItem. |

### Remarques

Cette méthode configure le [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/).

Format binaire XLS : AutoShow (Top10) est l'option native et la seule prise en charge.

XLSX (OpenXML) : Le format de fichier sous-jacent prend en charge Top10 AutoShow, mais l'interface utilisateur d'Excel 2007 et ultérieure ne l'expose que via le filtre Top10. Si la compatibilité XLS n'est pas requise, il est recommandé d'utiliser le filtre Top10 à la place.

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


