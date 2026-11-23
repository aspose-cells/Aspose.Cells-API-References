---
title: "ExternalConnection.PowerQueryFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Obtient la définition de la formule Power Query"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

Obtient la définition de la formule Power Query.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Charger un classeur existant avec des connexions de données pour démontrer PowerQueryFormula
            workbook = new Workbook("example.xlsx");
            
            // Accéder à une connexion existante (en supposant que le classeur possède au moins une connexion)
            if (workbook.DataConnections.Count > 0)
            {
                var connection = workbook.DataConnections[0];
                Console.WriteLine("Power Query Formula Demo:");
                Console.WriteLine($"Connection Name: {connection.Name}");
                
                // Accéder à la propriété PowerQueryFormula
                PowerQueryFormula powerQuery = connection.PowerQueryFormula;
                if (powerQuery != null)
                {
                    Console.WriteLine($"Formula Name: {powerQuery.Name}");
                    Console.WriteLine($"Formula Definition: {powerQuery.FormulaDefinition}");
                }
                else
                {
                    Console.WriteLine("No Power Query Formula found for this connection");
                }
            }
            else
            {
                Console.WriteLine("No data connections found in the workbook");
            }
            
            // Enregistrez le classeur
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


