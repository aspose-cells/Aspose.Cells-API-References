---
title: "StyleFlag.Alignments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración de alineación"
type: docs
url: /es/net/aspose.cells/styleflag/alignments/
---
## StyleFlag.Alignments property

Se aplicará la configuración de alineación.

```csharp
public bool Alignments { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyAlignmentsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer algún texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Cree un objeto de estilo y establezca las propiedades de alineación
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.RotationAngle = 45;

            // Crear una bandera de estilo y habilitar las propiedades de alineación
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Alignments = true;

            // Aplicar el estilo a la celda con la bandera de estilo
            cell.SetStyle(style, styleFlag);

            // Mostrar la configuración actual de alineación
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Modificar la bandera de estilo para deshabilitar las propiedades de alineación
            styleFlag.Alignments = false;
            
            // Crear un nuevo estilo con alineación diferente
            Style newStyle = workbook.CreateStyle();
            newStyle.HorizontalAlignment = TextAlignmentType.Right;
            newStyle.VerticalAlignment = TextAlignmentType.Top;
            newStyle.RotationAngle = 0;

            // Aplicar el nuevo estilo - las alineaciones no cambiarán porque la bandera está en false
            cell.SetStyle(newStyle, styleFlag);

            // Mostrar la configuración de alineación sin cambios
            Console.WriteLine("After applying new style with Alignments=false:");
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Guarda el libro de trabajo
            workbook.Save("StyleFlagAlignmentsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


