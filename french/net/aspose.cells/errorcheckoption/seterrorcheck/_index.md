---
title: "ErrorCheckOption.SetErrorCheck"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ErrorCheckOption. Définit si le type d'erreur donné sera vérifié"
type: docs
url: /fr/net/aspose.cells/errorcheckoption/seterrorcheck/
---
## ErrorCheckOption.SetErrorCheck method

Définit si le type d'erreur donné sera vérifié.

```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | Le type d'erreur peut être vérifié. |
| isCheck | Boolean | true si le type d'erreur donné doit être vérifié(triangle vert sera affiché pour la cellule si la vérification échoue). |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodSetErrorCheckWithErrorCheckTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Sample text for error checking");
            
            // Configurez les options de vérification d'erreurs
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
            
            // Démontrez SetErrorCheck avec différentes valeurs ErrorCheckType
            errorCheckOption.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, true);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            
            // Appliquer à toute la feuille de calcul
            errorCheckOption.AddRange(CellArea.CreateCellArea(0, 0, worksheet.Cells.MaxRow, worksheet.Cells.MaxDataColumn));
            
            workbook.Save("ErrorCheckExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


