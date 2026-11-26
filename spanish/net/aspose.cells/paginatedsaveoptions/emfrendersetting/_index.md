---
title: "PaginatedSaveOptions.EmfRenderSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Configuración para renderizar metarchivo Emf"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/emfrendersetting/
---
## PaginatedSaveOptions.EmfRenderSetting property

Configuración para renderizar metarchivo Emf.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Observaciones

Los metarchivos EMF identificados como "EMF+ Dual" pueden contener tanto registros EMF+ como registros EMF. Cualquiera de los tipos de registro puede usarse para renderizar la imagen, solo registros EMF+, o solo registros EMF. Cuando EmfPlusPrefer está configurado, los registros EMF+ se analizarán al renderizar la página; de lo contrario, solo se analizarán los registros EMF. El valor predeterminado es EmfOnly.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Crear imagen para la demostración de EMF
            worksheet.Pictures.Add(10, 10, "example.png");

            // Configurar opciones de guardado con ajustes EMF usando PdfSaveOptions
            PdfSaveOptions options = new PdfSaveOptions()
            {
                EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
            };

            // Guardar el libro de trabajo con ajustes EMF
            workbook.Save("EmfRenderSettingDemo.pdf", options);
        }
    }
}
```

### Ver también

* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


