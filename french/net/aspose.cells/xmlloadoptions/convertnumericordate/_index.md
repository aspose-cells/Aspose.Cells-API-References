---
title: "XmlLoadOptions.ConvertNumericOrDate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlLoadOptions. Indique si la conversion de la valeur du fichier xml en numérique ou en date est effectuée"
type: docs
url: /fr/net/aspose.cells/xmlloadoptions/convertnumericordate/
---
## XmlLoadOptions.ConvertNumericOrDate property

Indique si la conversion de la valeur du fichier xml en numérique ou en date.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            // Créez des options de chargement XML
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Définissez ConvertNumericOrDate sur true (par défaut)
            options.ConvertNumericOrDate = true;
            Workbook wb1 = new Workbook("input.xml", options);
            Cell cell1 = wb1.Worksheets[0].Cells["A1"];
            Console.WriteLine("With conversion (true): " + cell1.Value + " is type: " + cell1.Type);
            
            // Définissez ConvertNumericOrDate sur false
            options.ConvertNumericOrDate = false;
            Workbook wb2 = new Workbook("input.xml", options);
            Cell cell2 = wb2.Worksheets[0].Cells["A1"];
            Console.WriteLine("Without conversion (false): " + cell2.Value + " is type: " + cell2.Type);
            
            // Enregistrez les résultats
            wb1.Save("output_with_conversion.xlsx");
            wb2.Save("output_without_conversion.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


