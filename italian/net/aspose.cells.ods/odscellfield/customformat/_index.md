---
title: "OdsCellField.CustomFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsCellField. Rappresenta il formato personalizzato del valore del campo"
type: docs
url: /it/net/aspose.cells.ods/odscellfield/customformat/
---
## OdsCellField.CustomFormat property

Rappresenta il formato personalizzato del valore del campo.

```csharp
public string CustomFormat { get; set; }
```

### Esempi

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
            
            // Campo data con formato personalizzato
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            
            // Campo nome foglio senza formato personalizzato
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            
            // Campo titolo con formato personalizzato (dimostrando il formato stringa)
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

### Vedi anche

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


