---
title: "WebExtensionReference.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionReference. Obtient et définit l'identifiant associé à l'Office Addin au sein d'un fournisseur de catalogue. L'identifiant DOIT être unique au sein d'un fournisseur de catalogue"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionreference/id/
---
## WebExtensionReference.Id property

Obtient et définit l’identifiant associé à l’Office Add‑in au sein d’un fournisseur de catalogue. L’identifiant DOIT être unique au sein d’un fournisseur de catalogue.

```csharp
public string Id { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WebExtensionReferencePropertyIdDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            // Définition de la propriété Id et des autres propriétés de référence
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // Ajout de propriétés d'extension web
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            // Ajout de forme et liaison d'extension web
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            // Enregistrer et vérifier
            workbook.Save("web_extension_demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


