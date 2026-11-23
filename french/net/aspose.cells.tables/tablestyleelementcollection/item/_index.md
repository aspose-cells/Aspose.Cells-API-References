---
title: "TableStyleElementCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TableStyleElementCollection. Obtient un élément du style de tableau par l'index"
type: docs
url: /fr/net/aspose.cells.tables/tablestyleelementcollection/item/
---
## TableStyleElementCollection indexer (1 of 2)

Obtient un élément du style de tableau par l'index.

```csharp
public TableStyleElement this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

Renvoie l'objet [`TableStyleElement`](../../tablestyleelement/) 

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Pattern = BackgroundType.Solid;
            firstColStyle.BackgroundColor = System.Drawing.Color.LightBlue;

            string styleName = "CustomTableStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[elementIndex];
            element.SetElementStyle(firstColStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data");

            int tableIndex = workbook.Worksheets[0].ListObjects.Add(0, 0, 1, 0, true);
            ListObject table = workbook.Worksheets[0].ListObjects[tableIndex];
            table.ShowTableStyleFirstColumn = true;
            table.TableStyleName = styleName;

            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TableStyleElement](../../tablestyleelement/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## TableStyleElementCollection indexer (2 of 2)

Obtient l'élément du style de tableau par le type d'élément.

```csharp
public TableStyleElement this[TableStyleElementType type] { get; }
```

| Paramètre | Description |
| --- | --- |
| type | Le type d'élément. |

### Valeur de retour

Renvoie l'objet [`TableStyleElement`](../../tablestyleelement/) 

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer un style de tableau personnalisé
            string styleName = "CustomTableStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            // Accéder à la TableStyleElementCollection
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Ajouter un élément de style de tableau
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);

            try
            {
                // Accéder à la propriété Item en utilisant l'indexeur (qui utilise la propriété Item en interne)
                TableStyleElement element = elements[elementIndex];

                // Afficher les informations sur l'élément
                Console.WriteLine("Table Style Element Type: " + element.Type);
                Console.WriteLine("Element has been successfully accessed via Item property");

                // Enregistrez le classeur
                workbook.Save("TableStyleElementItemDemo.xlsx");
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

* class [TableStyleElement](../../tablestyleelement/)
* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


