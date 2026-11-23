---
title: "HtmlSaveOptions.MergeEmptyTdForcely"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si la fusion des éléments TD vides est forcée lors de l'exportation du fichier vers html. La taille du fichier html sera considérablement réduite après avoir défini la valeur sur true. La valeur par défaut est false. Si vous souhaitez importer le fichier html vers Excel ou exporter des lignes de grille parfaites lors de l'enregistrement du fichier en html, veuillez conserver la valeur par défaut."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/mergeemptytdforcely/
---
## HtmlSaveOptions.MergeEmptyTdForcely property

Indique si la fusion des éléments TD vides est forcée lors de l'exportation du fichier vers html. La taille du fichier html sera considérablement réduite après avoir défini la valeur sur true. La valeur par défaut est false. Si vous souhaitez importer le fichier html vers Excel ou exporter des lignes de grille parfaites lors de l'enregistrement du fichier en html, veuillez conserver la valeur par défaut.

```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdForcelyDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des cellules vides
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer quelques cellules vides dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            // B2 est intentionnellement laissé vide
            
            // Enregistrer avec MergeEmptyTdForcely activé
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.MergeEmptyTdForcely = true;
            workbook.Save("output_with_merge.html", options);
            
            // Enregistrer sans MergeEmptyTdForcely pour comparaison
            options.MergeEmptyTdForcely = false;
            workbook.Save("output_without_merge.html", options);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


