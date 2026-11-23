---
title: "XmlLoadOptions.IgnoreRootAttributes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlLoadOptions. Indique s'il faut ignorer les attributs de l'élément racine"
type: docs
url: /fr/net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

Indique si les attributs de l'élément racine sont ignorés.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
    {
        public static void Run()
        {
            // Créer des options de chargement XML et définir IgnoreRootAttributes
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;

            // Charger le fichier XML avec les options
            Workbook workbook = new Workbook("example.xml", options);

            // Accéder aux données du XML chargé
            string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
            Console.WriteLine("Cell AH8 value: " + cellValue);

            // Enregistrer au format XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


