---
title: "WebExtensionPropertyCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionPropertyCollection-metod. Lägger till webbutökningsegenskap"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionpropertycollection/add/
---
## WebExtensionPropertyCollection.Add method

Lägger till web extension‑egenskap.

```csharp
public int Add(string name, string value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på egenskapen. |
| värde | String | Värdet på egenskapen. |

### Returvärde

Index för tillagd egenskap.

### Exempel

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
            
            // Demonstrera Add-metoden med (String, String)-parametrar
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            workbook.Save("WebExtensionExample.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


