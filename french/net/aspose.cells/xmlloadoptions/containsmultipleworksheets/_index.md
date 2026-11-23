---
title: "XmlLoadOptions.ContainsMultipleWorksheets"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlLoadOptions. Indique si l'importation du xml se fait sous forme de plusieurs feuilles de calcul"
type: docs
url: /fr/net/aspose.cells/xmlloadoptions/containsmultipleworksheets/
---
## XmlLoadOptions.ContainsMultipleWorksheets property

Indique si l'importation du xml se fait en plusieurs feuilles de calcul.

```csharp
public bool ContainsMultipleWorksheets { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyContainsMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Créez un fichier Excel d'exemple avec plusieurs feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets[0].Cells["A1"].PutValue("Data from Sheet1");
            workbook.Worksheets[1].Cells["A1"].PutValue("Data from Sheet2");
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Enregistrez au format XML avec plusieurs feuilles de calcul
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output.xml", saveOptions);

            // Chargez le XML avec ContainsMultipleWorksheets=true
            XmlLoadOptions loadOptions = new XmlLoadOptions();
            loadOptions.ContainsMultipleWorksheets = true;
            Workbook loadedWorkbook = new Workbook("output.xml", loadOptions);

            // Vérifiez que les deux feuilles de calcul ont été chargées
            Console.WriteLine("Worksheet Count: " + loadedWorkbook.Worksheets.Count);
            Console.WriteLine("Sheet1 Data: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
            Console.WriteLine("Sheet2 Data: " + loadedWorkbook.Worksheets[1].Cells["A1"].StringValue);
        }
    }
}
```

### Voir aussi

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


