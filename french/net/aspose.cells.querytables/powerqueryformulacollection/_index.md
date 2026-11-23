---
title: "Classe PowerQueryFormulaCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaCollection classe. Représente toutes les formules Power Query dans les données mashup"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulacollection/
---
## PowerQueryFormulaCollection class

Représente toutes les formules Power Query dans les données mashup.

```csharp
public class PowerQueryFormulaCollection : CollectionBase<PowerQueryFormula>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.querytables/powerqueryformulacollection/item/) { get; } | Récupère [`PowerQueryFormula`](../powerqueryformula/) par l'index dans la liste. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormula) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormula, IComparer&lt;PowerQueryFormula&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PowerQueryFormula, IComparer&lt;PowerQueryFormula&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PowerQueryFormula) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormula[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormula[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PowerQueryFormula[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormula) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormula, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormula, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormula) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormula, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormula, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveBy](../../aspose.cells.querytables/powerqueryformulacollection/removeby/)(string) | Supprime la formule Power Query par son nom. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.QueryTables;
using System;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Crée un objet DataMashup
            DataMashup dataMashup = workbook.DataMashup;

            // Accède à la collection PowerQueryFormulas
            PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

            // Affiche le nombre de formules Power Query
            Console.WriteLine($"Number of Power Query Formulas: {powerQueryFormulas.Count}");

            // Exemple d'accès à une formule Power Query spécifique (si elle existe)
            if (powerQueryFormulas.Count > 0)
            {
                PowerQueryFormula firstFormula = powerQueryFormulas[0];
                Console.WriteLine($"First Power Query Formula: {firstFormula}");
            }

            // Enregistrez le classeur
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


