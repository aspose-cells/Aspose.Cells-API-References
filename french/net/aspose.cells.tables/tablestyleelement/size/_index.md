---
title: "TableStyleElement.Size"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TableStyleElement. Nombre de lignes ou de colonnes dans une seule bande de rayures. S'applique uniquement lorsque le type est firstRowStripe, secondRowStripe, firstColumnStripe ou secondColumnStripe"
type: docs
url: /fr/net/aspose.cells.tables/tablestyleelement/size/
---
## TableStyleElement.Size property

Nombre de lignes ou de colonnes dans une même bande de rayures. S’applique uniquement lorsque le type est firstRowStripe, secondRowStripe, firstColumnStripe ou secondColumnStripe.

```csharp
public int Size { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertySizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour créer une table
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Créer un tableau
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Créer un style de tableau en utilisant la collection de styles du classeur
            TableStyleCollection styleCollection = workbook.Worksheets.TableStyles;
            int styleIndex = styleCollection.AddTableStyle("CustomStyle");
            TableStyle style = styleCollection[styleIndex];
            table.TableStyleName = style.Name;

            // Ajouter des éléments de rayure pour démontrer la propriété Size
            style.TableStyleElements.Add(TableStyleElementType.FirstRowStripe);
            style.TableStyleElements.Add(TableStyleElementType.SecondRowStripe);

            // Accéder aux éléments de rayure
            TableStyleElement firstStripe = style.TableStyleElements[TableStyleElementType.FirstRowStripe];
            TableStyleElement secondStripe = style.TableStyleElements[TableStyleElementType.SecondRowStripe];

            // Afficher les valeurs actuelles de Size
            Console.WriteLine("Initial First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Initial Second Stripe Size: " + secondStripe.Size);

            // Modifier les tailles de rayure
            firstStripe.Size = 2;
            secondStripe.Size = 3;

            // Afficher les valeurs modifiées
            Console.WriteLine("Modified First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Modified Second Stripe Size: " + secondStripe.Size);

            // Enregistrer le classeur pour voir les effets
            workbook.Save("TableStyleElementSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


