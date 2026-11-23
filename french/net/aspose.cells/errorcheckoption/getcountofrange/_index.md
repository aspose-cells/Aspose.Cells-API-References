---
title: "ErrorCheckOption.GetCountOfRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ErrorCheckOption. Obtient le nombre de plages influencées par ce paramètre"
type: docs
url: /fr/net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

Obtient le nombre de plages influencées par ce paramètre.

```csharp
public int GetCountOfRange()
```

### Valeur de retour

le nombre de plages influencées par ce paramètre.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodGetCountOfRangeDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Obtenir la collection d'options de vérification d'erreurs
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;

            // Ajouter la première option de vérification d'erreurs
            int index1 = optsCollection.Add();
            ErrorCheckOption opts1 = optsCollection[index1];
            opts1.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts1.AddRange(CellArea.CreateCellArea("A1", "D2"));
            opts1.AddRange(CellArea.CreateCellArea("A3", "D3"));

            // Ajouter la deuxième option de vérification d'erreurs
            int index2 = optsCollection.Add();
            ErrorCheckOption opts2 = optsCollection[index2];
            opts2.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts2.AddRange(CellArea.CreateCellArea("A3", "D5"));

            // Démontrer la méthode GetCountOfRange
            Console.WriteLine("First option range count: " + opts1.GetCountOfRange());
            Console.WriteLine("Second option range count: " + opts2.GetCountOfRange());

            // Enregistrez le classeur
            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


