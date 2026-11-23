---
title: "LoadOptions.CheckDataValid"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Vérifiez si les données sont valides dans le fichier modèle"
type: docs
url: /fr/net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

Vérifier si les données sont valides dans le fichier modèle.

```csharp
public bool CheckDataValid { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckDataValidDemo
    {
        public static void Run()
        {
            // Créez des options de chargement avec CheckDataValid défini sur false
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CheckDataValid = false;

            // Chargez le classeur avec ces options
            Workbook workbook = new Workbook("example.xlsx", options);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une validation de données à des fins de démonstration
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Définir la plage de validation
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 10;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


