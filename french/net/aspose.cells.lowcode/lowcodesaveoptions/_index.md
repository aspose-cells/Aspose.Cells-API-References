---
title: "Classe LowCodeSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeSaveOptions. Options pour enregistrer les résultats générés de manière low‑code"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptions/
---
## LowCodeSaveOptions class

Options pour enregistrer les résultats générés de manière low‑code.

```csharp
public class LowCodeSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Obtient et définit le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, [`OutputStream`](./outputstream/) sera ignoré. |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Obtient et définit le flux pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, [`OutputFile`](./outputfile/) sera ignoré. |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | Obtient et définit le format d'enregistrement pour la sortie. En général, pour un processus spécifique en low‑code, seuls certains formats spécifiques sont autorisés. Veuillez spécifier le format correct pour le processus correspondant, sinon un résultat inattendu ou même une exception peut survenir. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et y placer des données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Créer des options d'enregistrement
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
            {
                OutputFile = "output.xlsx"
            };

            // Enregistrer le classeur en utilisant les options spécifiées
            workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
            
            Console.WriteLine("File saved successfully with LowCodeSaveOptions");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


