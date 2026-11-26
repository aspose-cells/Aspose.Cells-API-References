---
title: "LoadOptions.DefaultStyleSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo"
type: docs
url: /es/net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer opciones de carga con la configuración de estilo predeterminada
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
            
            // Crear una hoja de cálculo y obtener celdas
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Establecer valores para demostrar el estilo predeterminado
            cells["A1"].PutValue("Default Style Applied");
            cells["A2"].PutValue("Should have bottom alignment");
            
            // Crear una celda con estilo personalizado (para contrastar con el predeterminado)
            Cell customCell = cells["B1"];
            customCell.PutValue("Custom Style");
            Style customStyle = customCell.GetStyle();
            customStyle.VerticalAlignment = TextAlignmentType.Center;
            customCell.SetStyle(customStyle);
            
            // Guarda el libro de trabajo
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
            
            // Verificar los estilos
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("B1 Vertical Alignment: " + cells["B1"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Ver también

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


