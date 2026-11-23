---
title: "Worksheet.Replace"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Worksheet method. Remplace le texte de toutes les cellules par une nouvelle chaîne"
type: docs
url: /fr/net/aspose.cells/worksheet/replace/
---
## Worksheet.Replace method

Remplace le texte de toutes les cellules par une nouvelle chaîne.

```csharp
public int Replace(string oldString, string newString)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| oldString | String | Valeur de l'ancienne chaîne. |
| newString | String | Valeur de la nouvelle chaîne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("Hello Aspose");
            worksheet.Cells["A3"].PutValue("Hello Cells");
            
            // Ajouter une zone de texte avec du texte d'exemple
            worksheet.TextBoxes.Add(5, 0, 100, 50);
            worksheet.TextBoxes[0].Text = "Hello TextBox";
            
            // Définir l'en-tête et le pied de page
            worksheet.PageSetup.SetHeader(0, "Hello Header");
            worksheet.PageSetup.SetFooter(0, "Hello Footer");
            
            // Remplacer "Hello" par "Hi" dans tout le contenu
            string findText = "Hello";
            string replaceText = "Hi";
            worksheet.Replace(findText, replaceText);
            
            // Remplacer dans les en-têtes/pieds de page
            for (int i = 0; i < 3; i++)
            {
                if (worksheet.PageSetup.GetHeader(i) != null)
                    worksheet.PageSetup.SetHeader(i, worksheet.PageSetup.GetHeader(i).Replace(findText, replaceText));
                
                if (worksheet.PageSetup.GetFooter(i) != null)
                    worksheet.PageSetup.SetFooter(i, worksheet.PageSetup.GetFooter(i).Replace(findText, replaceText));
            }
            
            // Remplacer dans les zones de texte
            foreach (Aspose.Cells.Drawing.TextBox textBox in worksheet.TextBoxes)
            {
                if (textBox.Text != null)
                {
                    textBox.Text = textBox.Text.Replace(findText, replaceText);
                }
            }
            
            // Enregistrez le classeur
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


