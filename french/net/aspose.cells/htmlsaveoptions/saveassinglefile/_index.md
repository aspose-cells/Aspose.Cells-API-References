---
title: "HtmlSaveOptions.SaveAsSingleFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique s’il faut enregistrer le HTML en un seul fichier. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/saveassinglefile/
---
## HtmlSaveOptions.SaveAsSingleFile property

Indique s’il faut enregistrer le HTML en un seul fichier. La valeur par défaut est false.

```csharp
public bool SaveAsSingleFile { get; set; }
```

### Remarques

S’il y a plusieurs feuilles de calcul ou d’autres ressources nécessaires telles que des images dans le classeur, ces feuilles et ressources doivent généralement être enregistrées dans des fichiers séparés. Dans certains scénarios, l’utilisateur peut avoir besoin d’obtenir un seul fichier résultant, par exemple pour faciliter le transfert. Dans ce cas, l’utilisateur peut définir cette propriété sur true.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertySaveAsSingleFileDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Initialiser les options d’enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ExportPageHeaders = true;
            
            // Enregistrer le classeur en un seul fichier HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            // Vérifier que le fichier de sortie existe
            if (File.Exists(outputPath))
            {
                Console.WriteLine("HTML saved as single file successfully.");
            }
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


