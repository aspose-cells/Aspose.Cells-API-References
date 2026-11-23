---
title: "OdsCellField.CustomFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "OdsCellField propriété. Représente le format personnalisé de la valeur du champ"
type: docs
url: /fr/net/aspose.cells.ods/odscellfield/customformat/
---
## OdsCellField.CustomFormat property

Représente le format personnalisé de la valeur du champ.

```csharp
public string CustomFormat { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyCustomFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
            
            // Champ de date avec format personnalisé
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            
            // Champ de nom de feuille sans format personnalisé
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            
            // Champ de titre avec format personnalisé (démontrant le format de chaîne)
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, "Title Format: @");
            
            odsCellFields.UpdateFieldsValue();
            
            foreach (OdsCellField field in odsCellFields)
            {
                worksheet.Cells[field.Row, field.Column].PutValue(
                    $"Type: {field.FieldType}, Format: {field.CustomFormat ?? "None"}");
            }
            
            workbook.Save("OdsCellFieldCustomFormatDemo.ods");
        }
    }
}
```

### Voir aussi

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


