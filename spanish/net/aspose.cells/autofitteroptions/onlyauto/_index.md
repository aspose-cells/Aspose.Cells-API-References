---
title: "AutoFitterOptions.OnlyAuto"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFitterOptions. Indica si solo se ajustan las filas cuya altura no está personalizada"
type: docs
url: /es/net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Indica si solo se ajustan las filas cuya altura no está personalizada.

```csharp
public bool OnlyAuto { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyOnlyAutoDemo
    {
        public static void Run()
        {
            // Crear opciones de carga y establecer la propiedad OnlyAuto
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = new AutoFitterOptions();
            loadOptions.AutoFitterOptions.OnlyAuto = true;

            // Cargar libro de trabajo con opciones de ajuste automático
            Workbook workbook = new Workbook("example.xml", loadOptions);
            
            // Demostrar el ajuste automático comprobando el ancho de columna
            Console.WriteLine("Column width after auto-fit: " + 
                workbook.Worksheets[0].Cells.GetColumnWidthPixel(0));
            
            // Guardar y recargar para verificar la persistencia
            workbook.Save("example_output.xlsx");
            Workbook reloaded = new Workbook("example_output.xlsx");
            Console.WriteLine("Reloaded column width: " + 
                reloaded.Worksheets[0].Cells.GetColumnWidthPixel(0));
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


