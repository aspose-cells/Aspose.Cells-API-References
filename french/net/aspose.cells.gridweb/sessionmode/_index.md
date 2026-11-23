---
title: "Énumération SessionMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.GridWeb.SessionMode. Représente le mode de session de la grille"
type: docs
url: /fr/net/aspose.cells.gridweb/sessionmode/
---
## SessionMode enumeration

Représente le mode de session de la grille.

```csharp
public enum SessionMode
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Session | `0` | Utilise la session système pour stocker/récupérer automatiquement les données de la feuille de la grille. |
| ViewState | `1` | Utilise le viewstate de la page pour stocker/récupérer automatiquement les données de la feuille de la grille. |
| Custom | `2` | Utilise l'événement LoadCustomData pour charger manuellement les données de la feuille de la grille. Et utilise l'événement SheetDataUpdated pour enregistrer les données de la feuille de la grille. |
| File | `3` | Utilise le fichier système pour stocker/récupérer automatiquement les données de la feuille de la grille, l'utilisateur doit définir SessionStorePath pour spécifier le répertoire du fichier. |

### Voir aussi

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


