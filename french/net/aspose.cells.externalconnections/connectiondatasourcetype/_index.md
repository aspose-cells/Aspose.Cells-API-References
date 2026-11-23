---
title: "Enum ConnectionDataSourceType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ExternalConnections.ConnectionDataSourceType enum. Spécifie le type de source de base de données externe"
type: docs
url: /fr/net/aspose.cells.externalconnections/connectiondatasourcetype/
---
## ConnectionDataSourceType enumeration

Spécifie le type de source de base de données externe

```csharp
public enum ConnectionDataSourceType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| ODBCBasedSource | `1` | Source basée sur ODBC |
| DAOBasedSource | `2` | Source basée sur DAO |
| FileBasedDataBaseSource | `3` | Source de base de données basée sur un fichier |
| WebQuery | `4` | Requête Web |
| OLEDBBasedSource | `5` | Source basée sur OLE DB |
| TextBasedSource | `6` | Source basée sur du texte |
| ADORecordSet | `7` | Ensemble d'enregistrements ADO |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | Source de données OLE DB créée par le modèle de données de la feuille de calcul. |
| DataFeedDataModel | `101` | Source de données de flux créée par le modèle de données de la feuille de calcul. |
| WorksheetDataModel | `102` | Source de données de feuille de calcul créée par le modèle de données de la feuille de calcul. |
| Table | `102` | Source de données de feuille de calcul créée par le modèle de données de la feuille de calcul. |
| TextDataModel | `103` | Source de données texte créée par le modèle de données de la feuille de calcul. |
| Unknown | `255` | Source de données texte créée par le modèle de données de la feuille de calcul. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassConnectionDataSourceTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(2000);

            // Créer un tableau croisé dynamique en utilisant les données de la feuille de calcul
            var pivotTable = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            
            // Obtenir la connexion et démontrer ConnectionDataSourceType
            var conn = sheet.PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Class Type: " + conn.ClassType);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Enregistrez le classeur
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


