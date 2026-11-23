---
title: "XmlLoadOptions.DateFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlLoadOptions. Obtient et définit le format de la valeur de date"
type: docs
url: /fr/net/aspose.cells/xmlloadoptions/dateformat/
---
## XmlLoadOptions.DateFormat property

Obtient et définit le format de la valeur de date.

```csharp
public string DateFormat { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Créez une instance de XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Définir le format de date pour analyser les dates à partir du XML
            options.DateFormat = "yyyy-MM-dd";
            options.ConvertNumericOrDate = true;

            // Chargez un fichier XML dans un classeur en utilisant les options spécifiées
            Workbook workbook = new Workbook("input.xml", options);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Afficher certaines cellules pour démontrer le formatage des dates
            Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);

            // Enregistrez le classeur dans un nouveau fichier
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


