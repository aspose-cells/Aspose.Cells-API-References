---
title: "ExternalConnection.SourceType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Obtient ou définit le type de source de données de la connexion externe"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/sourcetype/
---
## ExternalConnection.SourceType property

Obtient ou définit le type DataSource de la connexion externe.

```csharp
public ConnectionDataSourceType SourceType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertySourceTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez une feuille de calcul et créez un tableau croisé dynamique
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B3"].PutValue(2000);
            
            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            
            // Obtenir la connexion externe
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Démontrez la propriété SourceType
            Console.WriteLine("Connection Source Type: " + conn.SourceType);
            
            // Modifiez les propriétés de la connexion
            conn.Name = "TestConnection";
            conn.SourceType = ConnectionDataSourceType.OLEDBDataModel;
            
            // Affichez les propriétés modifiées
            Console.WriteLine("Modified Connection Name: " + conn.Name);
            Console.WriteLine("Modified Source Type: " + conn.SourceType);
        }
    }
}
```

### Voir aussi

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


