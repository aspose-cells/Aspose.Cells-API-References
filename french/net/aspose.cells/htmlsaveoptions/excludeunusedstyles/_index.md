---
title: "HtmlSaveOptions.ExcludeUnusedStyles"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si les styles inutilisés sont exclus. Pour les fichiers HTML générés, exclure les styles inutilisés peut réduire la taille du fichier sans affecter l’aspect visuel. Ainsi, la valeur par défaut de cette propriété est true. Si l’utilisateur doit conserver tous les styles dans le classeur pour le HTML généré, par exemple dans le cas où il doit restaurer le classeur à partir du HTML généré ultérieurement, veuillez définir cette propriété sur false."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/excludeunusedstyles/
---
## HtmlSaveOptions.ExcludeUnusedStyles property

Indique s'il faut exclure les styles inutilisés. Pour les fichiers html générés, exclure les styles inutilisés peut réduire la taille du fichier sans affecter les effets visuels. Ainsi, la valeur par défaut de cette propriété est true. Si l'utilisateur doit conserver tous les styles dans le classeur pour le html généré (par exemple dans le cas où l'utilisateur doit restaurer le classeur à partir du html généré ultérieurement), veuillez définir cette propriété sur false.

```csharp
public bool ExcludeUnusedStyles { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExcludeUnusedStylesDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des données d’exemple avec différents styles
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.Value = "Styled text";
            Style style1 = cell1.GetStyle();
            style1.Font.Color = Color.Red;
            style1.Font.IsBold = true;
            cell1.SetStyle(style1);

            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.Value = "Different style";
            Style style2 = cell2.GetStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            cell2.SetStyle(style2);

            // Configurer les options d’enregistrement HTML pour exclure les styles inutilisés
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExcludeUnusedStyles = true;

            // Enregistrer le classeur avec les options HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with ExcludeUnusedStyles=true");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


