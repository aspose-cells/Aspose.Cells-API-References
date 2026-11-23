---
title: "XmlDataBinding.Url"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlDataBinding. Obtient l'URL source de cette liaison de données"
type: docs
url: /fr/net/aspose.cells/xmldatabinding/url/
---
## XmlDataBinding.Url property

Obtient l'URL source de cette liaison de données.

```csharp
public string Url { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class XmlDataBindingPropertyUrlDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter deux feuilles de calcul
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");

            // Ajouter des objets de liste et des cartes XML
            ListObject list1 = workbook.Worksheets[0].ListObjects[0];
            ListObject list2 = workbook.Worksheets[1].ListObjects[0];
            
            // Obtenir les URL de liaison de données XML (Url est en lecture seule)
            string url1 = list1.XmlMap.DataBinding.Url;
            string url2 = list2.XmlMap.DataBinding.Url;

            // Afficher les URL
            Console.WriteLine("Sheet1 ListObject XML URL: " + url1);
            Console.WriteLine("Sheet2 ListObject XML URL: " + url2);

            // Enregistrez le classeur
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


