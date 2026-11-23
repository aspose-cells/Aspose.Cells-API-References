---
title: "Range.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient l'objet Cell dans cette plage"
type: docs
url: /fr/net/aspose.cells/range/item/
---
## Range indexer

Obtient l'objet [`Cell`](../../cell/) dans cette plage.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| Paramètre | Description |
| --- | --- |
| rowOffset | Décalage de ligne dans cette plage, indexé à zéro. |
| columnOffset | Décalage de colonne dans cette plage, indexé à zéro. |

### Valeur de retour

[`Cell`](../../cell/) object.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangePropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple
            DataTable dt = new DataTable();
            dt.Columns.Add("Id", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Rows.Add(1001, "Item 1");
            dt.Rows.Add(1002, "Item 2");

            // Créez une plage et démontrez la propriété Item
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B3");
            
            // Définissez les en-têtes en utilisant la propriété Item
            range[0, 0].PutValue("Id");
            range[0, 1].PutValue("Name");

            // Remplissez les données en utilisant la propriété Item
            for (int i = 0; i < dt.Rows.Count; i++)
            {
                range[i + 1, 0].PutValue(dt.Rows[i]["Id"]);
                range[i + 1, 1].PutValue(dt.Rows[i]["Name"]);
            }

            // Formatez la ligne d'en-tête en utilisant la propriété Item
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.FromArgb(0, 176, 80);
            range[0, 0].SetStyle(style);
            range[0, 1].SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("RangePropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


