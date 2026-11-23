---
title: "XmlLoadOptions.StartCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlLoadOptions. Obtient et définit la cellule de départ"
type: docs
url: /fr/net/aspose.cells/xmlloadoptions/startcell/
---
## XmlLoadOptions.StartCell property

Obtient et définit la cellule de départ.

```csharp
public string StartCell { get; set; }
```

### Remarques

Fonctionne uniquement lorsque le fichier n'est pas speadsheetML ou que le mappage du xml vers Excel n'est pas activé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Créez une instance de XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Définir la cellule de départ pour l'importation des données XML
            options.StartCell = "B2";

            // Chargez un fichier XML dans un classeur en utilisant les options spécifiées
            Workbook workbook = new Workbook("input.xml", options);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Affichez la valeur de la cellule de départ pour démontrer la propriété
            Console.WriteLine("Value at start cell (B2): " + worksheet.Cells["B2"].Value);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


