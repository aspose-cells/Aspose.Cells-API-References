---
title: "PowerQueryFormulaParameter.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormulaParameter. Obtient le type de la formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulaparameter/type/
---
## PowerQueryFormulaParameter.Type property

Obtient le type de la formule Power Query.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Comme nous ne pouvons pas créer directement un PowerQueryFormulaParameter sans connaître les paramètres requis du constructeur,
                // nous démontrerons l'accès à la propriété Type via les paramètres d'une table de requête existante
                Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
                
                // Dans un scénario réel, vous accéderiez à cela depuis une table de requête existante
                // À des fins de démonstration, nous montrerons comment vérifier le type si vous aviez une instance
                PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
                
                if (parameter != null)
                {
                    // Affichez la valeur de la propriété Type (propriété en lecture seule)
                    Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
                    
                    // Afficher les valeurs d'énumération possibles
                    Console.WriteLine("Possible PowerQueryFormulaType values:");
                    foreach (PowerQueryFormulaType type in Enum.GetValues(typeof(PowerQueryFormulaType)))
                    {
                        Console.WriteLine($"- {type}");
                    }
                }
                else
                {
                    Console.WriteLine("No PowerQueryFormulaParameter instance available for demonstration.");
                }
                
                // Enregistrez le classeur
                workbook.Save("TypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


