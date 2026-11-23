---
title: "Enum OLEDBCommandType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.ExternalConnections.OLEDBCommandType. Spécifie le type de commande OLE DB"
type: docs
url: /fr/net/aspose.cells.externalconnections/oledbcommandtype/
---
## OLEDBCommandType enumeration

Spécifie le type de commande OLE DB.

```csharp
public enum OLEDBCommandType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Le type de commande n'est pas spécifié. |
| CubeName | `1` | Spécifie un nom de cube |
| SqlStatement | `2` | Spécifie une instruction SQL |
| TableName | `3` | Spécifie un nom de table |
| DefaultInformation | `4` | Spécifie que des informations par défaut ont été données, et il revient au fournisseur de les interpréter. |
| WebBasedList | `5` | Spécifie une requête qui s'adresse à un fournisseur de données de liste basé sur le Web. |
| TableCollection | `6` | Spécifie la liste des tables. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassOLEDBCommandTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Obtenir la connexion externe
            ExternalConnectionCollection connections = workbook.DataConnections;
            ExternalConnection conn = connections[0];
            
            // Démontrer l'utilisation de OLEDBCommandType
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command Type: " + conn.CommandType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Modifier le type de commande et démontrer
            conn.CommandType = OLEDBCommandType.TableName;
            Console.WriteLine("\nAfter changing CommandType:");
            Console.WriteLine("Command Type: " + conn.CommandType);
            
            // Enregistrez le classeur
            workbook.Save("OLEDBCommandTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


