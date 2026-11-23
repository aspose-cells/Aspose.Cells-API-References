---
title: "Classe PowerQueryFormulaParameter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.QueryTables.PowerQueryFormulaParameter. Représente le paramètre de la formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulaparameter/
---
## PowerQueryFormulaParameter class

Représente le paramètre de la formule Power Query.

```csharp
public class PowerQueryFormulaParameter : PowerQueryFormula
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Obtient et définit la description de la formule Power Query.(Hérité de [`PowerQueryFormula`](../powerqueryformula/).) |
| override [FormulaDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/) { get; } | Obtient la définition du paramètre. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Obtient le nom du groupe qui contient cette formule Power Query.(Hérité de [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Obtient et définit le nom de la formule Power Query.(Hérité de [`PowerQueryFormula`](../powerqueryformula/).) |
| [ParameterDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/) { get; } | (**Obsolète.**) Obtient la définition du paramètre. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Obtient tous les éléments de la formule Power Query.(Hérité de [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulaparameter/type/) { get; } | Obtient le type de la formule Power Query. |
| [Value](../../aspose.cells.querytables/powerqueryformulaparameter/value/) { get; set; } | Obtient la valeur du paramètre. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterDemo
    {
        public static void PowerQueryFormulaParameterExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Accédez à la propriété DataMashup du classeur
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Accédez à la propriété PowerQueryFormulas
                PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Accédez à la propriété PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Exemple d'utilisation : Parcourez les PowerQueryFormulas
                foreach (PowerQueryFormula formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Exemple d'utilisation : parcourir PowerQueryFormulaParameters
                foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
                {
                    // Afficher les détails du paramètre
                    Console.WriteLine("Parameter Name: " + para.Name);
                    Console.WriteLine("Parameter Value: " + para.Value);

                    Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
                }
            }
            

            // Enregistrez le classeur
            workbook.Save("PowerQueryFormulaParameterExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


