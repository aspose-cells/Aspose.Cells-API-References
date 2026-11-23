---
title: "DataMashup.PowerQueryFormulaParameters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataMashup. Obtient les paramètres de formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/datamashup/powerqueryformulaparameters/
---
## DataMashup.PowerQueryFormulaParameters property

Obtient les paramètres de formule Power Query.

```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété DataMashup.PowerQueryFormulas. Cette propriété sera supprimée 12 mois plus tard à compter de novembre 2024. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulaParametersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la propriété DataMashup
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Accéder à PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                // Afficher le nombre de paramètres
                Console.WriteLine($"Number of parameters: {parameters.Count}");

                // Itérer à travers les paramètres s'ils existent
                foreach (PowerQueryFormulaParameter parameter in parameters)
                {
                    Console.WriteLine($"Parameter Name: {parameter.Name}, Value: {parameter.Value}");
                }
            }

            // Enregistrez le classeur
            workbook.Save("DataMashupDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


