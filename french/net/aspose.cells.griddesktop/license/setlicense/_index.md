---
title: "License.SetLicense"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode License. Licence le composant"
type: docs
url: /fr/net/aspose.cells.griddesktop/license/setlicense/
---
## SetLicense(Stream) {#setlicense}

Licence le composant.

```csharp
public void SetLicense(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Un flux qui contient la licence. |

### Remarques

Utilisez cette méthode pour charger une licence à partir d'un flux.

### Exemples

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)
```

### Voir aussi

* class [License](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## SetLicense(string) {#setlicense_1}

Licence le composant.

```csharp
public void SetLicense(string licenseName)
```

### Remarques

Essaie de trouver la licence aux emplacements suivants :

1. Chemin explicite.

2. Le dossier qui contient l'assembly du composant Aspose.

3. Le dossier qui contient l'assembly appelant du client.

4. Le dossier qui contient l'assembly d'entrée (démarrage).

5. Une ressource intégrée dans l'assembly appelant du client.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Chemin explicite.

2. Une ressource intégrée dans l'assembly appelant du client.

### Exemples

Dans cet exemple, une tentative sera faite pour trouver un fichier de licence nommé MyLicense.lic dans le dossier contenant le composant, dans le dossier contenant l'assembly appelant, dans le dossier de l'assembly d'entrée, puis dans les ressources incorporées de l'assembly appelant.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

Peut être un nom de fichier complet ou court ou le nom d'une ressource incorporée. Utilisez une chaîne vide pour passer en mode d'évaluation.

### Voir aussi

* class [License](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


