---
title: "LowCodeLoadOptions.InputFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeLoadOptions. Obtient et définit le chemin du fichier du modèle si nécessaire"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodeloadoptions/inputfile/
---
## LowCodeLoadOptions.InputFile property

Obtient et définit le fichier (avec le chemin si nécessaire) du modèle.

```csharp
public string InputFile { get; set; }
```

### Remarques

Lors de la définition d'un chemin non nul et non vide pour cette propriété, la valeur précédemment définie pour [`InputStream`](../inputstream/) sera ignorée.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeLoadOptionsPropertyInputFileDemo
    {
        public static void Run()
        {
            // Créez et enregistrez un fichier modèle d'exemple
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
            const string templatePath = "LowCodeTemplate.xlsx";
            templateWorkbook.Save(templatePath);

            // Initialisez LowCodeLoadOptions et démontrez la propriété InputFile
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);

            // Définissez la propriété InputFile pour utiliser notre modèle
            loadOptions.InputFile = templatePath;
            Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);

            // Chargez le classeur en utilisant le fichier modèle spécifié
            Workbook workbook = new Workbook(loadOptions.InputFile);
            
            // Modifiez le modèle chargé
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);

            // Enregistrer le classeur modifié
            workbook.Save("PropertyInputFileDemo_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


