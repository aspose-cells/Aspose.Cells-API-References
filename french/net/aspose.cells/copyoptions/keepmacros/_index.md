---
title: "CopyOptions.KeepMacros"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CopyOptions. Indique si les macros sont conservées"
type: docs
url: /fr/net/aspose.cells/copyoptions/keepmacros/
---
## CopyOptions.KeepMacros property

Indique s'il faut conserver les macros ;

```csharp
public bool KeepMacros { get; set; }
```

### Remarques

Uniquement pour la copie du classeur.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyKeepMacrosDemo
    {
        public static void Run()
        {
            // Créer un classeur source avec des macros (en utilisant un fichier modèle contenant des macros)
            Workbook srcWorkbook = new Workbook("macros_template.xlsm");
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Macro-enabled source");

            // Créer le classeur de destination
            Workbook destWorkbook = new Workbook();
            
            // Définir les options de copie avec KeepMacros à true
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;

            // Copier la feuille de calcul avec des macros
            destWorkbook.Worksheets[0].Copy(srcSheet, options);

            // Enregistrer le résultat
            destWorkbook.Save("KeepMacrosExample.xlsm");
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


