---
title: "PivotTable.GetSourceDataConnections"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Obtient les sources de données de connexion externes"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/getsourcedataconnections/
---
## PivotTable.GetSourceDataConnections method

Obtient les sources de données de connexion externes.

```csharp
public ExternalConnection[] GetSourceDataConnections()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            
            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Obtenir les connexions de données source
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Afficher les informations de connexion
            if (connections.Length > 0)
            {
                ExternalConnection conn = connections[0];
                Console.WriteLine("Connection Name: " + conn.Name);
                Console.WriteLine("Class Type: " + conn.ClassType);
                Console.WriteLine("Source Type: " + conn.SourceType);
                Console.WriteLine("Command: " + conn.Command);
            }
            
            // Enregistrez le classeur
            workbook.Save("PivotTableSourceConnections.xlsx");
        }
    }
}
```

### Voir aussi

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


