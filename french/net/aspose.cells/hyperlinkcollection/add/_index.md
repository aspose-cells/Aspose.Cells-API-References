---
title: "HyperlinkCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode HyperlinkCollection. Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules"
type: docs
url: /fr/net/aspose.cells/hyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de la plage d'hyperliens. |
| firstColumn | Int32 | Première colonne de la plage d'hyperliens. |
| totalRows | Int32 | Nombre de lignes dans cette plage d'hyperliens. |
| totalColumns | Int32 | Nombre de colonnes de cette plage d'hyperliens. |
| address | String | Adresse de l'hyperlien. |

### Valeur de retour

[`Hyperlink`](../../hyperlink/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un hyperlien en utilisant les coordonnées ligne/colonne et les dimensions
            worksheet.Hyperlinks.Add(0, 0, 1, 1, "http://www.aspose.com");
            worksheet.Hyperlinks.Add(1, 0, 1, 1, "c:\\book1.xls");
            
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_1}

Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule. |
| totalRows | Int32 | Nombre de lignes dans cette plage d'hyperliens. |
| totalColumns | Int32 | Nombre de colonnes de cette plage d'hyperliens. |
| address | String | Adresse de l'hyperlien. |

### Valeur de retour

[`Hyperlink`](../../hyperlink/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Ajouter un hyperlien à la cellule A1 avec l'adresse "www.aspose.com"
            hyperlinks.Add("A1", 1, 1, "www.aspose.com");
            
            // Afficher l'adresse de l'hyperlien
            Console.WriteLine("Hyperlink Address: " + worksheet.Cells["A1"].StringValue);
            
            // Modifier le texte affiché
            worksheet.Cells["A1"].PutValue("Click Here");
            Console.WriteLine("Display Text: " + hyperlinks[0].TextToDisplay);
            
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, string, string) {#add_2}

Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startCellName | String | La cellule en haut à gauche de la plage. |
| endCellName | String | La cellule en bas à droite de la plage. |
| address | String | Adresse de l'hyperlien. |
| textToDisplay | String | Le texte à afficher pour l'hyperlien spécifié. |
| screenTip | String | Le texte screenTip pour le lien hypertexte spécifié. |

### Valeur de retour

[`Hyperlink`](../../hyperlink/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Démontrer la méthode Add avec les paramètres (String, String, String, String, String)
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            workbook.Save("HyperlinkCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


