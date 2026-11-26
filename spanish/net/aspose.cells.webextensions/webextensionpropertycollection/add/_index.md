---
title: "WebExtensionPropertyCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WebExtensionPropertyCollection. Añade una propiedad de extensión web"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionpropertycollection/add/
---
## WebExtensionPropertyCollection.Add method

Agrega una propiedad de extensión web.

```csharp
public int Add(string name, string value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad. |
| valor | String | El valor de la propiedad. |

### Valor de retorno

El índice de la propiedad añadida.

### Ejemplos

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
            
            // Demostrar el método Add con parámetros (String, String)
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            workbook.Save("WebExtensionExample.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


