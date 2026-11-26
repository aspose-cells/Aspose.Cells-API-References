---
title: "StyleFlag.Rotation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración Rotation"
type: docs
url: /es/net/aspose.cells/styleflag/rotation/
---
## StyleFlag.Rotation property

Se aplicará la configuración de rotación.

```csharp
public bool Rotation { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyRotationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer algún texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Rotated Text");

            // Obtener el estilo de la celda
            Style style = workbook.CreateStyle();

            // Establecer nuevo valor de rotación (45 grados)
            style.RotationAngle = 45;

            // Mostrar valor de rotación actual
            Console.WriteLine("Current Rotation value: " + cell.GetStyle().RotationAngle);            

            // Crear una bandera de estilo y habilitar la bandera de rotación
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Rotation = true;

            // Aplicar el estilo con rotación a la celda
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("after setting style, rotation value: " + cell.GetStyle().RotationAngle);
           
            // Guardar el resultado
            workbook.Save("PropertyRotationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


