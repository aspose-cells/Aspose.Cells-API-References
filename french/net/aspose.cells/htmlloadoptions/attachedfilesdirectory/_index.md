---
title: "HtmlLoadOptions.AttachedFilesDirectory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Le répertoire où les fichiers joints seront enregistrés"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

Le répertoire où les fichiers joints seront enregistrés.

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété HtmlLoadOptions.StreamProvider. Cette propriété sera supprimée 12 mois plus tard depuis décembre 2014. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Créer une instance de HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Définir le répertoire pour les fichiers joints
            options.AttachedFilesDirectory = "C:\\AttachedFiles";

            // Charger un fichier HTML dans un classeur en utilisant les options spécifiées
            Workbook workbook = new Workbook("input.html", options);

            // Enregistrez le classeur dans un fichier Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


