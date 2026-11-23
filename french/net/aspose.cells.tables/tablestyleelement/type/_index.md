---
title: "TableStyleElement.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TableStyleElement. Obtient le type de l'élément"
type: docs
url: /fr/net/aspose.cells.tables/tablestyleelement/type/
---
## TableStyleElement.Type property

Obtient le type de l’élément.

```csharp
public TableStyleElementType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour créer une table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Créer un tableau
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Obtenir le style de tableau (en utilisant le nom du style au lieu d'en créer un nouveau)
            string styleName = table.TableStyleName;
            TableStyle style = workbook.Worksheets.TableStyles[styleName];

            // Accéder aux éléments de style de tableau
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.HeaderRow];

            // Afficher le type actuel de l'élément
            Console.WriteLine("Current Type value: " + element.Type);

            // Remarque : la propriété Type est en lecture seule, donc nous ne pouvons pas la définir
            // element.Type = TableStyleElementType.TotalRow; // Cela provoquerait une erreur de compilation

            // Démontrer comment différents types d'éléments affectent le tableau
            Console.WriteLine("\nAvailable table style elements:");
            foreach (TableStyleElementType type in Enum.GetValues(typeof(TableStyleElementType)))
            {
                try
                {
                    TableStyleElement testElement = style.TableStyleElements[type];
                    Console.WriteLine($"Element type {type} exists in this style");
                }
                catch
                {
                    Console.WriteLine($"Element type {type} not available in this style");
                }
            }

            // Enregistrez le classeur
            workbook.Save("TableStyleElementTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


