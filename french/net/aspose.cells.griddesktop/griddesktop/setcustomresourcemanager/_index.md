---
title: "GridDesktop.SetCustomResourceManager"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridDesktop. Définit le gestionnaire de ressources personnalisé pour implémenter la localisation définie par l'utilisateur."
type: docs
url: /fr/net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

Définir un gestionnaire de ressources personnalisé pour implémenter la localisation définie par l'utilisateur

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| customResourceManager | ResourceManager | le gestionnaire de ressources personnalisé. |

### Remarques

Pour créer un fichier de ressources personnalisé, veuillez suivre le format dans GridDesktopResource.resx.

### Exemples

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


