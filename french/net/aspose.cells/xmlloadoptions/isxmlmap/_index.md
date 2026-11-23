---
title: "XmlLoadOptions.IsXmlMap"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlLoadOptions. Indique si le mappage du xml vers Excel est activé. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/xmlloadoptions/isxmlmap/
---
## XmlLoadOptions.IsXmlMap property

Indique si le mappage du XML vers Excel est activé. La valeur par défaut est false.

```csharp
public bool IsXmlMap { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIsXmlMapDemo
    {
        public static void Run()
        {
            // Créez une instance de XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Activer le mappage XML lors du chargement du fichier
            options.IsXmlMap = true;

            // Chargez un fichier XML dans un classeur en utilisant les options spécifiées
            Workbook workbook = new Workbook("sample.xml", options);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Afficher certaines données du XML chargé pour démontrer le mappage réussi
            Console.WriteLine("Data from loaded XML:");
            Console.WriteLine(worksheet.Cells["A1"].StringValue);
            Console.WriteLine(worksheet.Cells["A2"].StringValue);

            // Enregistrer le classeur dans un nouveau fichier Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


