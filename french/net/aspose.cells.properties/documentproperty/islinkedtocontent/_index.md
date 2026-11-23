---
title: "DocumentProperty.IsLinkedToContent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocumentProperty. Indique si cette propriété est liée au contenu"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/islinkedtocontent/
---
## DocumentProperty.IsLinkedToContent property

Indique si cette propriété est liée au contenu

```csharp
public bool IsLinkedToContent { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyIsLinkedToContentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple aux cellules
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Company Name";
            worksheet.Cells["B1"].Value = "Company Address";

            // Créez des propriétés de document personnalisées liées
            workbook.CustomDocumentProperties.AddLinkToContent("Company", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Address", "B1");

            // Obtenez et vérifiez la propriété IsLinkedToContent
            DocumentProperty companyProp = workbook.CustomDocumentProperties["Company"];
            Console.WriteLine($"Is 'Company' property linked to content: {companyProp.IsLinkedToContent}");
            Console.WriteLine($"Linked source: {companyProp.Source}");
            Console.WriteLine($"Current value: {companyProp.Value}");

            // Mettez à jour la valeur de la cellule et rafraîchissez les propriétés liées
            worksheet.Cells["A1"].Value = "Updated Company Name";
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Vérifier que la propriété a été mise à jour
            Console.WriteLine($"Updated value: {companyProp.Value}");

            // Enregistrez le classeur
            workbook.Save("LinkedPropertiesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


