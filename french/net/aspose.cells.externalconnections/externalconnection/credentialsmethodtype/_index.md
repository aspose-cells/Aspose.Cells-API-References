---
title: "ExternalConnection.CredentialsMethodType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Spécifie la méthode d’authentification à utiliser lors de l’établissement ou du rétablissement de la connexion"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/credentialsmethodtype/
---
## ExternalConnection.CredentialsMethodType property

Spécifie la méthode d’authentification à utiliser lors de l’établissement (ou du ré‑établissement) de la connexion.

```csharp
public CredentialsMethodType CredentialsMethodType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyCredentialsMethodTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Ajoutez une feuille de calcul et créez un tableau croisé dynamique pour établir une connexion externe
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Product");
                sheet.Cells["B1"].PutValue("Sales");
                sheet.Cells["A2"].PutValue("Apple");
                sheet.Cells["B2"].PutValue(1000);
                sheet.Cells["A3"].PutValue("Banana");
                sheet.Cells["B3"].PutValue(2000);

                // Créez un tableau croisé dynamique qui aura une connexion externe
                int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

                // Obtenez la connexion externe depuis le tableau croisé dynamique
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Affichez la valeur actuelle de CredentialsMethodType
                Console.WriteLine("Initial CredentialsMethodType: " + connection.CredentialsMethodType);

                // Démontrez la définition de la propriété (car elle est en lecture‑écriture)
                connection.CredentialsMethodType = CredentialsMethodType.Stored;
                Console.WriteLine("Updated CredentialsMethodType: " + connection.CredentialsMethodType);

                // Définissez une autre valeur pour démontrer
                connection.CredentialsMethodType = CredentialsMethodType.Integrated;
                Console.WriteLine("Changed CredentialsMethodType: " + connection.CredentialsMethodType);

                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("CredentialsMethodTypeDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


