---
title: "Énumération WebExtensionStoreType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.WebExtensions.WebExtensionStoreType. Représente le type de magasin de l'extension web"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionstoretype/
---
## WebExtensionStoreType enumeration

Représente le type de magasin de l'extension web.

```csharp
public enum WebExtensionStoreType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| OMEX | `0` | Spécifie que le type de magasin est Office.com. |
| SPCatalog | `1` | Spécifie que le type de magasin est le catalogue d'entreprise SharePoint. |
| SPApp | `2` | Spécifie que le type de magasin est une application web SharePoint. |
| Exchange | `3` | Spécifie que le type de magasin est un serveur Exchange. |
| FileSystem | `4` | Spécifie que le type de magasin est un partage de système de fichiers. |
| Registry | `5` | Spécifie que le type de magasin est le registre système. |
| ExCatalog | `6` | Spécifie que le type de magasin est le déploiement centralisé via Exchange. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionStoreTypeDemo
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
            
            webExt.Properties.Add("sku", "\"peoplebar-giant\"");
            webExt.Properties.Add("theme", "\"giant-redwhiteblack\"");
            webExt.Properties.Add("shape", "\"muscle-people\"");
            webExt.Properties.Add("layout-element-title", "\"NUMBERS ABOUT THE APP\"");
            
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            workbook.Save("WebExtensionStoreTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


