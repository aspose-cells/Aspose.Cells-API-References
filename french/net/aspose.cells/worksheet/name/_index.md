---
title: "Worksheet.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient ou définit le nom de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Obtient ou définit le nom de la feuille de calcul.

```csharp
public string Name { get; set; }
```

### Remarques

La longueur maximale du nom d’une feuille est de 31 caractères. Vous ne pouvez pas attribuer le même nom (insensible à la casse) à deux feuilles de calcul. Par exemple, vous ne pouvez pas définir "SheetName1" pour la première feuille et définir "SHEETNAME1" pour la deuxième feuille.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et définissez son nom
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Ajoutez une nouvelle feuille de calcul avec un nom spécifique
            Worksheet newSheet = workbook.Worksheets.Add("ReportSheet");
            
            // Affichez les noms de toutes les feuilles de calcul
            Console.WriteLine("Worksheet Names:");
            foreach (Worksheet ws in workbook.Worksheets)
            {
                Console.WriteLine(ws.Name);
            }
            
            // Enregistrez le classeur
            workbook.Save("WorksheetNamesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


