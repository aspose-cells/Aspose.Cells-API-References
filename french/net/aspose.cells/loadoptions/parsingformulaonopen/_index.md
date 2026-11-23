---
title: "LoadOptions.ParsingFormulaOnOpen"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Indique si l'analyse de la formule est effectuée lors de la lecture du fichier"
type: docs
url: /fr/net/aspose.cells/loadoptions/parsingformulaonopen/
---
## LoadOptions.ParsingFormulaOnOpen property

Indique s'il faut analyser la formule lors de la lecture du fichier.

```csharp
public bool ParsingFormulaOnOpen { get; set; }
```

### Remarques

S'applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm et Xlsm car les formules dans les fichiers sont stockées sous forme de chaîne de formule.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingFormulaOnOpenDemo
    {
        public static void Run()
        {
            // Créer des options de chargement
            LoadOptions loadOptions = new LoadOptions();
            
            // Définir ParsingFormulaOnOpen sur false pour ignorer l'analyse des formules lors du chargement
            loadOptions.ParsingFormulaOnOpen = false;
            
            // Chargez le classeur avec les options spécifiées
            Workbook workbook = new Workbook("example.xlsm", loadOptions);
            
            // Accéder à la feuille de calcul et démontrer que l'analyse des formules a été ignorée
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Console.WriteLine("Cell A1 formula: " + cell.Formula);
            Console.WriteLine("Cell A1 value: " + cell.Value);
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


