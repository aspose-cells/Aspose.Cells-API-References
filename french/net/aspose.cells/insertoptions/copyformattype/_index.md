---
title: "InsertOptions.CopyFormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété InsertOptions."
type: docs
url: /fr/net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyCopyFormatTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir les valeurs et le formatage à des fins de démonstration
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");

            // Créez InsertOptions et définissez CopyFormatType
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.SameAsAbove;

            // Insérer une ligne avec le formatage ci-dessus
            worksheet.Cells.InsertRows(2, 1, options);

            // Enregistrer le résultat
            workbook.Save("InsertWithFormatting.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


