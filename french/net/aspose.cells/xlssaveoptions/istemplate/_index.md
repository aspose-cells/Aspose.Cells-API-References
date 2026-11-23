---
title: "XlsSaveOptions.IsTemplate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "XlsSaveOptions propriété. Indique si l'enregistrement d'un fichier modèle"
type: docs
url: /fr/net/aspose.cells/xlssaveoptions/istemplate/
---
## XlsSaveOptions.IsTemplate property

Indique si l'enregistrement d'un fichier modèle.

```csharp
[Obsolete("Use XlsSaveOptions(SaveFormat.Xlt) when it is template, otherwise use XlsSaveOptions().")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsTemplate { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez créer XlsSaveOptions avec le format d'enregistrement correspondant (xlt pour true et xls pour false). Cette méthode sera supprimée 12 mois plus tard, depuis août 2020. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyIsTemplateDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Template");
            
            // Enregistrer comme fichier modèle
            string outputPath = "output_template.xlt";
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.IsTemplate = true;
            
            using (FileStream fs = File.Create(outputPath))
            {
                workbook.Save(fs, saveOptions);
            }
            
            // Vérifier le format du fichier enregistré
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("File format: " + loadedWorkbook.FileFormat);
        }
    }
}
```

### Voir aussi

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


