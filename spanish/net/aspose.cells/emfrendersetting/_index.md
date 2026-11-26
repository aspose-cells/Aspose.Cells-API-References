---
title: "Enum EmfRenderSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.EmfRenderSetting. Configuración para renderizar metarchivo Emf"
type: docs
url: /es/net/aspose.cells/emfrendersetting/
---
## EmfRenderSetting enumeration

Configuración para renderizar metarchivo Emf.

```csharp
public enum EmfRenderSetting
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| EmfOnly | `0` | Solo renderizando registros Emf. |
| EmfPlusPrefer | `1` | Preferir renderizar registros EmfPlus. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue("Using EmfOnly setting");

            // Crear opciones de imagen con la configuración de renderizado EMF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                EmfRenderSetting = EmfRenderSetting.EmfOnly
            };

            // Crear un renderizado de hoja con las opciones
            SheetRender render = new SheetRender(worksheet, options);

            // Guardar la primera página como imagen EMF
            render.ToImage(0, "EmfRenderSettingDemo.emf");

            Console.WriteLine("EMF file created successfully with EmfOnly setting.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


