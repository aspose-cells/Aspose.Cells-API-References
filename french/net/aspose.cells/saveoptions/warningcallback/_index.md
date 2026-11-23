---
title: "SaveOptions.WarningCallback"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Obtient ou définit le rappel d’avertissement"
type: docs
url: /fr/net/aspose.cells/saveoptions/warningcallback/
---
## SaveOptions.WarningCallback property

Obtient ou définit le rappel d'avertissement.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data");

            // Créer des options d'enregistrement
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Définir un rappel d’avertissement personnalisé
            saveOptions.WarningCallback = new CustomWarningCallback();

            // Cela générera un avertissement concernant une fonctionnalité non prise en charge au format HTML
            worksheet.PageSetup.PrintTitleRows = "$1:$1";

            // Enregistrer avec des options pouvant déclencher des avertissements
            workbook.Save("WarningCallbackDemo.html", saveOptions);
        }
    }

    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Gérer l’avertissement - dans ce cas, l’afficher simplement
            Console.WriteLine($"Warning: {warningInfo.Description}");
            Console.WriteLine($"Warning type: {warningInfo.WarningType}");
        }
    }
}
```

### Voir aussi

* interface [IWarningCallback](../../iwarningcallback/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


