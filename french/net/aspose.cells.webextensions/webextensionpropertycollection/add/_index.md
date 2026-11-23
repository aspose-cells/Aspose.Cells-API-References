---
title: "WebExtensionPropertyCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WebExtensionPropertyCollection. Ajoute une propriété d'extension web"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionpropertycollection/add/
---
## WebExtensionPropertyCollection.Add method

Ajoute une propriété d'extension web.

```csharp
public int Add(string name, string value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété. |
| valeur | String | La valeur de la propriété. |

### Valeur de retour

L'index de la propriété ajoutée.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // Démontrer la méthode Add avec des paramètres (String, String)
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            workbook.Save("WebExtensionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


