---
title: "Workbook.GetStyleInPool"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Récupère le style dans le pool de styles. Tous les styles du classeur seront rassemblés dans un pool. Il n’y a qu’un simple indice de référence dans les cellules"
type: docs
url: /fr/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Obtient le style dans le pool de styles. Tous les styles du classeur seront rassemblés dans un pool. Il n'y a qu'un simple index de référence dans les cellules.

```csharp
public Style GetStyleInPool(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'indice. |

### Valeur de retour

Le style dans le pool correspond à l’indice donné, peut être nul.

### Remarques

Si le style retourné est modifié, le style de toutes les cellules (qui font référence à ce style) sera modifié.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetStyleInPoolWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Accéder à la première feuille de calcul et ajouter des données d'exemple
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123.45);
            ws.Cells["A3"].PutValue(DateTime.Now);
            
            // Appliquer certains styles
            Style style1 = wb.CreateStyle();
            style1.Custom = "$#,##0.00";
            ws.Cells["A2"].SetStyle(style1);
            
            Style style2 = wb.CreateStyle();
            style2.Custom = "yyyy-mm-dd";
            ws.Cells["A3"].SetStyle(style2);
            
            // Enregistrer dans le flux mémoire
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                
                // Recharger le classeur depuis le flux
                ms.Position = 0;
                Workbook reloadWb = new Workbook(ms);
                
                // Obtenir et afficher les styles du pool de styles
                int count = reloadWb.CountOfStylesInPool;
                Console.WriteLine($"Styles in pool: {count}");
                
                for (int i = 0; i < count; i++)
                {
                    Style style = reloadWb.GetStyleInPool(i);
                    Console.WriteLine($"Style {i}: CustomFormat={style.Custom}");
                }
            }
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


