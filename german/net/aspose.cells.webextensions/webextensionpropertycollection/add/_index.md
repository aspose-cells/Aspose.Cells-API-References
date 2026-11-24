---
title: "WebExtensionPropertyCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionPropertyCollection-Methode. Fügt eine WebExtension-Eigenschaft hinzu"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionpropertycollection/add/
---
## WebExtensionPropertyCollection.Add method

Fügt eine Web‑Extension‑Eigenschaft hinzu.

```csharp
public int Add(string name, string value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Eigenschaft. |
| Wert | String | Der Wert der Eigenschaft. |

### Rückgabewert

Der Index der hinzugefügten Eigenschaft.

### Beispiele

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
            
            // Demonstriere die Add-Methode mit (String, String)-Parametern
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            workbook.Save("WebExtensionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


