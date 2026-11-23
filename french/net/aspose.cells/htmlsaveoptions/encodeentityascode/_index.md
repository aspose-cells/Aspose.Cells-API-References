---
title: "HtmlSaveOptions.EncodeEntityAsCode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si les entités de caractères HTML sont remplacées par un code décimal. Par exemple, nbsp est remplacé par 160. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/encodeentityascode/
---
## HtmlSaveOptions.EncodeEntityAsCode property

Indique si les entités de caractères html sont remplacées par un code décimal. (par ex. "&amp;nbsp;" est remplacé par "&amp;#160;"). La valeur par défaut est false.

```csharp
public bool EncodeEntityAsCode { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec des caractères spéciaux
            worksheet.Cells["A1"].PutValue("Sample & Text");
            worksheet.Cells["A2"].PutValue("Another <Test> String");
            worksheet.Cells["A3"].PutValue("Price: $100");

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Afficher la valeur actuelle de EncodeEntityAsCode
            Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);

            // Définir EncodeEntityAsCode sur true
            options.EncodeEntityAsCode = true;

            // Enregistrer avec les entités encodées en code
            workbook.Save("HtmlWithEncodedEntities.html", options);

            // Définir EncodeEntityAsCode sur false
            options.EncodeEntityAsCode = false;

            // Enregistrer les entités telles quelles
            workbook.Save("HtmlWithRawEntities.html", options);

            // Comparer les fichiers de sortie
            Console.WriteLine("Files created:");
            Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
            Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


