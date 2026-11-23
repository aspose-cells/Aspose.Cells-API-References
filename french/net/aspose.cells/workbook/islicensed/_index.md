---
title: "Workbook.IsLicensed"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Indique si la licence est définie"
type: docs
url: /fr/net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

Indique si la licence est définie.

```csharp
public bool IsLicensed { get; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsLicensedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Définir quelques propriétés de base pour démontrer que le workbook est utilisé
            wb.Worksheets[0].Name = "Sheet1";
            wb.Worksheets[0].Cells[0, 0].PutValue("Sample Data");
            
            // Vérifier si le classeur est sous licence
            Console.WriteLine($"IsLicensed: {wb.IsLicensed}");
            
            // Démontrer un comportement différent en fonction de l'état de la licence
            if (wb.IsLicensed)
            {
                Console.WriteLine("Running in licensed mode - full features available");
            }
            else
            {
                Console.WriteLine("Running in evaluation mode - watermarks will appear");
            }

            // Enregistrer dans le memory stream pour démontrer la fonctionnalité
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                Console.WriteLine($"Workbook saved successfully (Size: {ms.Length} bytes)");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


