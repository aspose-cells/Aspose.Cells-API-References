---
title: "CustomDocumentPropertyCollection.UpdateLinkedPropertyValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CustomDocumentPropertyCollection. Met à jour les valeurs de toutes les propriétés personnalisées qui sont liées au contenu en utilisant la valeur de la cellule de la plage liée pour mettre à jour la valeur de la propriété personnalisée"
type: docs
url: /fr/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

Met à jour les valeurs de toutes les propriétés personnalisées qui sont liées au contenu (utilise la valeur de cellule de la plage liée pour mettre à jour la valeur de la propriété personnalisée).

```csharp
public void UpdateLinkedPropertyValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedPropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des données aux cellules qui seront liées aux propriétés personnalisées
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "InitialValue1";
            worksheet.Cells["B1"].Value = "InitialValue2";

            // Ajouter des propriétés personnalisées liées
            workbook.CustomDocumentProperties.AddLinkToContent("CompanyName", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Department", "B1");

            // Mettre à jour les valeurs des cellules
            worksheet.Cells["A1"].Value = "UpdatedValue1";
            worksheet.Cells["B1"].Value = "UpdatedValue2";

            // Mettre à jour les valeurs des propriétés liées
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Afficher les valeurs des propriétés mises à jour
            Console.WriteLine("CompanyName: " + workbook.CustomDocumentProperties["CompanyName"].Value);
            Console.WriteLine("Department: " + workbook.CustomDocumentProperties["Department"].Value);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


