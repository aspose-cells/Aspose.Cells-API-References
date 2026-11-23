---
title: "MainWeb.SessionMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "MainWeb propriété. Obtient ou définit le mode de session de la grille"
type: docs
url: /fr/net/aspose.cells.gridweb/mainweb/sessionmode/
---
## MainWeb.SessionMode property

Obtient ou définit le mode de session de la grille.

```csharp
public SessionMode SessionMode { get; set; }
```

### Remarques

Il existe 4 types de mode de session : 1. Session (par défaut) : Utilisez la session système pour stocker les données de la feuille. En général, asp.net utilise l’état de session InProc. La grille prend également en charge l’état de session "StateServer" hors processus et l’état de session SQLServer. 2. ViewState : Utilisez le viewstate de la page pour stocker les données de la feuille. 3. Custom : Utilisez les événements LoadCustomData et SheetDataUpdated pour stocker/récupérer les données de la feuille. 4. File : stockez/récupérez les données de la feuille dans SessionStorePath. C’est la méthode recommandée et permet de garder le fichier en permanence. Lors de l’utilisation de SessionMode.ViewState, la grille stockera certaines données dans le viewstate de la page. Cela réduira l’utilisation de la mémoire du serveur, mais la taille de la page sera plus grande et cela affectera les performances globales.

### Exemples

```csharp
[C#]
	GridWeb1.SessionMode = SessionMode.ViewState;
	
[Visual Basic]
	GridWeb1.SessionMode = SessionMode.ViewState
```

### Voir aussi

* enum [SessionMode](../../sessionmode/)
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


