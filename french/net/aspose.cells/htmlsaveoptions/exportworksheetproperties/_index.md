---
title: "HtmlSaveOptions.ExportWorksheetProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indiquant si l'exportation des propriétés de la feuille de calcul est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportworksheetproperties/
---
## HtmlSaveOptions.ExportWorksheetProperties property

Indiquant si l'exportation des propriétés de la feuille de calcul est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans excel, veuillez conserver la valeur par défaut.

```csharp
public bool ExportWorksheetProperties { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetPropertiesDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Définir les options d'enregistrement HTML avec ExportWorksheetProperties désactivé
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportWorksheetProperties = false;
            
            // Enregistrer avec les propriétés de la feuille de calcul désactivées
            workbook.Save("output_without_worksheet_props.html", options);

            // Activer l'exportation des propriétés de la feuille de calcul
            options.ExportWorksheetProperties = true;
            
            // Enregistrer avec les propriétés de la feuille de calcul activées
            workbook.Save("output_with_worksheet_props.html", options);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


