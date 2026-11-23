---
title: "DocxSaveOptions.SaveAsEditableShaps"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocxSaveOptions. Enregistrer tous les objets de dessin objecgts en tant que formes éditables dans le fichier word. Ainsi, vous pouvez les modifier dans Word"
type: docs
url: /fr/net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

Enregistrer tous les objets de dessin objecgts en tant que formes éditables dans le fichier word. Ainsi, vous pouvez les modifier dans Word.

```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [`SaveAsEditableShapes`](../saveaseditableshapes/). Cette propriété sera supprimée 6 mois plus tard, depuis mai 2025. Aspose s\'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
    {
        public static void Run()
        {
            // Créer un objet classeur et ouvrir le fichier Excel modèle
            Workbook workbook = new Workbook("example.xlsx");

            // Initialiser DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            
            // Définir la propriété SaveAsEditableShaps sur true
            saveOptions.SaveAsEditableShaps = true;

            // Enregistrer le classeur en DOCX avec les options spécifiées
            workbook.Save("example.docx", saveOptions);
        }
    }
}
```

### Voir aussi

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


