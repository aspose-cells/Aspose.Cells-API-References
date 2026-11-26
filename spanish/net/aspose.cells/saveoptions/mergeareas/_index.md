---
title: "SaveOptions.MergeAreas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo"
type: docs
url: /es/net/aspose.cells/saveoptions/mergeareas/
---
## SaveOptions.MergeAreas property

Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.

```csharp
public bool MergeAreas { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyMergeAreasDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar datos y crear celdas combinadas
            worksheet.Cells["A1"].PutValue("Merged Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Combinar celdas A1:B1
            worksheet.Cells.Merge(0, 0, 1, 2);

            // Crear opciones de guardado con MergeAreas habilitado
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MergeAreas = true;

            // Guardar con optimización de áreas combinadas
            workbook.Save("MergeAreasDemo.xlsx", saveOptions);
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


