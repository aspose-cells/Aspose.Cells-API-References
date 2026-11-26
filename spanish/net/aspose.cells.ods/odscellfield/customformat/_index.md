---
title: "OdsCellField.CustomFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsCellField. Representa el formato personalizado del valor del campo"
type: docs
url: /es/net/aspose.cells.ods/odscellfield/customformat/
---
## OdsCellField.CustomFormat property

Representa el formato personalizado del valor del campo.

```csharp
public string CustomFormat { get; set; }
```

### Ejemplos

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
            
            // Campo de fecha con formato personalizado
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            
            // Campo de nombre de hoja sin formato personalizado
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            
            // Campo de título con formato personalizado (demostrando formato de cadena)
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

### Ver también

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


