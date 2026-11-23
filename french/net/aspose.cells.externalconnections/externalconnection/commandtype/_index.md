---
title: "ExternalConnection.CommandType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Spécifie le type de commande OLE DB. 1. La requête spécifie un nom de cube 2. La requête spécifie une instruction SQL 3. La requête spécifie un nom de table 4. La requête indique que des informations par défaut ont été fournies et il appartient au fournisseur de les interpréter 5. La requête porte sur un fournisseur de données de liste basé sur le Web"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

Spécifie le type de commande OLE DB. 1. Query spécifie un nom de cube 2. Query spécifie une instruction SQL 3. Query spécifie un nom de table 4. Query spécifie que des informations par défaut ont été fournies, et il revient au fournisseur de les interpréter. 5. Query porte sur un fournisseur de données de liste basé sur le web.

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];

            // Obtenir la connexion externe
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Démontrer la propriété CommandType
            Console.WriteLine("Original CommandType: " + conn.CommandType);
            
            // Modifier et afficher CommandType
            conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
            Console.WriteLine("Modified CommandType: " + conn.CommandType);
            
            // Enregistrez le classeur
            workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


