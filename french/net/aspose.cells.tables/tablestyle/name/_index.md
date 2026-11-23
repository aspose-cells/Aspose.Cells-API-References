---
title: "TableStyle.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TableStyle. Récupère le nom du style de tableau"
type: docs
url: /fr/net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

Obtient le nom du style de tableau.

```csharp
public string Name { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accédez à la collection des styles de tableau
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            try
            {
                // Obtenir le premier style de tableau de la collection
                TableStyle tableStyle = tableStyles[0];

                // Afficher la valeur de la propriété Name
                Console.WriteLine("Table Style Name: " + tableStyle.Name);

                // Démontrer l'accès à la propriété en lecture seule
                string styleName = tableStyle.Name;
                Console.WriteLine("Retrieved style name: " + styleName);

                // Montrer que nous pouvons utiliser le nom pour référencer le style
                Console.WriteLine("This table style can be referenced by name: " + tableStyle.Name);

                // Enregistrez le classeur
                workbook.Save("TableStyleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


