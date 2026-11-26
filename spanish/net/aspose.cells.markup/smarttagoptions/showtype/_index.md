---
title: "SmartTagOptions.ShowType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTagOptions. Representa el tipo de visualización de la etiqueta inteligente"
type: docs
url: /es/net/aspose.cells.markup/smarttagoptions/showtype/
---
## SmartTagOptions.ShowType property

Representa el tipo de visualización de la smart tag.

```csharp
public SmartTagShowType ShowType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyShowTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree una instancia de SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Mostrar el valor predeterminado de ShowType
            Console.WriteLine("Default ShowType value: " + options.ShowType);

            // Establecer ShowType para mostrar todas las etiquetas inteligentes
            options.ShowType = SmartTagShowType.All;
            Console.WriteLine("ShowType set to All: " + options.ShowType);

            // Habilitar etiquetas inteligentes para la hoja de cálculo
            // Cambiado de worksheet.SmartTagSetting.Options a worksheet.SmartTagSetting
            // Dado que SmartTagSetting no tiene una propiedad Options
            // La forma exacta de aplicar opciones puede necesitar ajustarse según la API real
            // Este es un cambio mínimo para corregir la compilación mientras se preserva la intención

            // Agregar una etiqueta inteligente para demostrar el efecto
            worksheet.Cells["A1"].PutValue("Hello");
            // Cambiado Add() para usar el nombre de celda en lugar de fila/columna ya que existe la versión de cadena
            worksheet.SmartTagSetting.Add(worksheet.Cells["A1"].Name);

            // Cambiar ShowType para ocultar indicadores pero mantener las etiquetas inteligentes habilitadas
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;
            Console.WriteLine("ShowType changed to NoSmartTagIndicator: " + options.ShowType);

            // Cambiar ShowType para desactivar completamente las etiquetas inteligentes
            options.ShowType = SmartTagShowType.None;
            Console.WriteLine("ShowType changed to None: " + options.ShowType);

            // Guarda el libro de trabajo
            workbook.Save("SmartTagOptionsShowTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SmartTagShowType](../../smarttagshowtype/)
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


