---
title: "SpreadsheetML2003SaveOptions.LimitAsXls"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SpreadsheetML2003SaveOptions. Limite en tant que xls : l'index maximal de ligne est 65535 et l'index maximal de colonne est 255"
type: docs
url: /fr/net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

Limite en tant que xls, l'index maximal de ligne est 65535 et l'index maximal de colonne est 255.

```csharp
public bool LimitAsXls { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyLimitAsXlsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Accéder aux cellules et créer une plage
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "C5");
            range.Name = "TestRange";
            
            // Enregistrer avec LimitAsXls = true
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            
            // Enregistrer en tant que SpreadsheetML avec les limites XLS
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with LimitAsXls=true");
        }
    }
}
```

### Voir aussi

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


