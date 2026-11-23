---
title: "Protection.AllowFormattingCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Représente si le formatage des cellules est autorisé sur une feuille protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowformattingcell/
---
## Protection.AllowFormattingCell property

Représente si le formatage des cellules est autorisé sur une feuille de calcul protégée.

```csharp
public bool AllowFormattingCell { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Activer la protection de la feuille
            Protection protection = worksheet.Protection;
            
            // Définir diverses propriétés de protection en utilisant un indicateur
            int flag = 0x40; // Only AllowFormattingCell flag is set
            protection.AllowFormattingCell = (flag & 0x40) != 0;

            // Vérifiez le paramètre
            Console.WriteLine("AllowFormattingCell is set to: " + protection.AllowFormattingCell);

            // Enregistrez le classeur
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


