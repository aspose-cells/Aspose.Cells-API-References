---
title: "PowerQueryFormulaCollection.RemoveBy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PowerQueryFormulaCollection. Supprimez la formule Power Query par son nom"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulacollection/removeby/
---
## PowerQueryFormulaCollection.RemoveBy method

Supprime la formule Power Query par son nom.

```csharp
public void RemoveBy(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la formule Power Query. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaCollectionMethodRemoveByWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la PowerQueryFormulaCollection (en supposant qu'elle existe dans le classeur)
                PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
                
                // Ajoutez une formule d'exemple à supprimer (cela proviendrait normalement de données existantes)
                string formulaName = "SampleFormula";
                
                // Appelez RemoveBy avec le nom de la formule
                powerQueryFormulas.RemoveBy(formulaName);
                
                Console.WriteLine($"Formula '{formulaName}' removed successfully");
                
                // Enregistrez le classeur
                workbook.Save("RemoveByWithStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RemoveBy demonstration: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


