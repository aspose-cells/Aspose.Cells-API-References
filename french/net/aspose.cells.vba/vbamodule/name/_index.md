---
title: "VbaModule.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaModule. Obtient et définit le nom du module"
type: docs
url: /fr/net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

Obtient et définit le nom du module.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();

            // Ajoutez une feuille de calcul et récupérez son module VBA
            Worksheet sheet = wb.Worksheets[0];
            int moduleIndex = wb.VbaProject.Modules.Add(sheet);
            VbaModule module = wb.VbaProject.Modules[moduleIndex];

            // Définissez le nom du module
            module.Name = "Sheet1";

            // Ajoutez du code VBA simple au module
            string vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n" +
                             "    MsgBox \"Sheet name: \" & Me.Name\r\n" +
                             "End Sub\r\n";
            module.Codes = vbaCode;

            // Enregistrez dans un flux mémoire (à des fins de démonstration)
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsm);
            }
        }
    }
}
```

### Voir aussi

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


