---
title: "Font.IsSuperscript"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient ou définit une valeur indiquant si la police est en exposant"
type: docs
url: /fr/net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

Obtient ou définit une valeur indiquant si la police est en exposant.

```csharp
public bool IsSuperscript { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSuperscriptDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez du texte à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Normal Text Superscript Text");
            
            // Formatez une partie du texte en exposant
            FontSetting setting = cell.Characters(12, 11);
            setting.Font.IsSuperscript = true;
            
            // Enregistrez le classeur
            workbook.Save("FontIsSuperscriptDemo.xlsx");
            
            // Vérifier le paramètre de superindice
            Console.WriteLine("IsSuperscript property: " + setting.Font.IsSuperscript);
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


