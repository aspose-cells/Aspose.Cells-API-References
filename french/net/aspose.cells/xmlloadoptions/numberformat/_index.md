---
title: "XmlLoadOptions.NumberFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlLoadOptions. Obtient et définit le format de la valeur numérique"
type: docs
url: /fr/net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

Obtient et définit le format de la valeur numérique.

```csharp
public string NumberFormat { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Créez une instance de XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Définir la propriété NumberFormat pour afficher les nombres avec 2 décimales
            options.NumberFormat = "0.00";

            // Chargez un fichier XML dans un classeur en utilisant les options spécifiées
            Workbook workbook = new Workbook("input.xml", options);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir quelques valeurs numériques pour démontrer le formatage des nombres
            worksheet.Cells["A1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(45.678);
            worksheet.Cells["A3"].PutValue(0.5);

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


