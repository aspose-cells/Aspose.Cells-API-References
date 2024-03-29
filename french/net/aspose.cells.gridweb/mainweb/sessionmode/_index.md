---
title: SessionMode
second_title: Référence de l'API Aspose.Cells pour .NET
description: Obtient ou définit le mode de session de la grille. Il existe 4 types de mode de session  1. Session par défaut  utiliser la session système pour stocker les données de la feuille. Généralement asp.net utilise létat de session InProc. La grille prend également en charge StateServer out process session state et SQLServer session state. 2. ViewState  utilisez létat daffichage de la page pour stocker les données de la feuille. 3. Personnalisé  utilisez les événements LoadCustomData et SheetDataUpdated pour stocker/récupérer les données de la feuille. 4. Fichier  stocker/récupérer les données de la feuille dans SessionStorePath.
type: docs
weight: 810
url: /fr/net/aspose.cells.gridweb/mainweb/sessionmode/
---
## MainWeb.SessionMode property

Obtient ou définit le mode de session de la grille. Il existe 4 types de mode de session : 1. Session (par défaut) : utiliser la session système pour stocker les données de la feuille. Généralement, asp.net utilise l'état de session InProc. La grille prend également en charge "StateServer" out process session state et SQLServer session state. 2. ViewState : utilisez l'état d'affichage de la page pour stocker les données de la feuille. 3. Personnalisé : utilisez les événements LoadCustomData et SheetDataUpdated pour stocker/récupérer les données de la feuille. 4. Fichier : stocker/récupérer les données de la feuille dans SessionStorePath.

```csharp
public SessionMode SessionMode { get; set; }
```

### Remarques

Lors de l'utilisation de SessionMode.ViewState, la grille stockera les données des feuilles dans l'état d'affichage de la page. Cela réduira l'utilisation de la mémoire du serveur, mais la taille de la page sera plus grande et cela aura un impact sur les performances globales.

### Exemples

```csharp
[C#]
	GridWeb1.SessionMode = SessionMode.ViewState;
	
[Visual Basic]
	GridWeb1.SessionMode = SessionMode.ViewState
```

### Voir également

* enum [SessionMode](../../sessionmode)
* class [MainWeb](../../mainweb)
* espace de noms [Aspose.Cells.GridWeb](../../mainweb)
* Assemblée [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
