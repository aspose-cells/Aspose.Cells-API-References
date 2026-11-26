---
title: "JsonSaveOptions.ToExcelStruct"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Indica si se convierte a una estructura json del archivo Excel"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

Indica si se convierte a la estructura json del archivo Excel.

```csharp
public bool ToExcelStruct { get; set; }
```

### Observaciones

Solo para convertir el rango a JSON.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyToExcelStructDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Crear un rango para exportar
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            // Configurar opciones de guardado JSON con ToExcelStruct
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;

            // Exporta rango a JSON
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


