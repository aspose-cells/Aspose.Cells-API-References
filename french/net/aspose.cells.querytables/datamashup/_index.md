---
title: "Classe DataMashup"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.QueryTables.DataMashup. Représente les données de mashup"
type: docs
url: /fr/net/aspose.cells.querytables/datamashup/
---
## DataMashup class

Représente les données mashup.

```csharp
public class DataMashup
```

## Propriétés

| Nom | Description |
| --- | --- |
| [PowerQueryFormulaParameters](../../aspose.cells.querytables/datamashup/powerqueryformulaparameters/) { get; } | (**Obsolète.**) Obtient les paramètres de formule Power Query. |
| [PowerQueryFormulas](../../aspose.cells.querytables/datamashup/powerqueryformulas/) { get; } | Récupère toutes les formules Power Query. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class DataMashupDemo
    {
        public static void DataMashupExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la propriété DataMashup du classeur
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null )
            {
                // Accédez à la propriété PowerQueryFormulas
                var powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Accédez à la propriété PowerQueryFormulaParameters
                var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Exemple d'utilisation : Parcourez les PowerQueryFormulas
                foreach (var formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Exemple d'utilisation : parcourir PowerQueryFormulaParameters
                foreach (var parameter in powerQueryFormulaParameters)
                {
                    Console.WriteLine(parameter.Name);
                }
            }
            

            // Enregistrez le classeur
            workbook.Save("DataMashupExample.xlsx");
            workbook.Save("DataMashupExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


