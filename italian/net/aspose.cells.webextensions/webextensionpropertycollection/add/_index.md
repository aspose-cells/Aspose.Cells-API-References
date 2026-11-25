---
title: "WebExtensionPropertyCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WebExtensionPropertyCollection. Aggiunge la proprietà web extension"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionpropertycollection/add/
---
## WebExtensionPropertyCollection.Add method

Aggiunge una proprietà dell'estensione web.

```csharp
public int Add(string name, string value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà. |
| valore | String | Il valore della proprietà. |

### Valore di ritorno

L'indice della proprietà aggiunta.

### Esempi

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
            
            // Dimostrare il metodo Add con parametri (String, String)
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            workbook.Save("WebExtensionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


