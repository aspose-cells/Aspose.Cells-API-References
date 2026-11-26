---
title: "Style.ParentStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene el estilo padre de este estilo"
type: docs
url: /es/net/aspose.cells/style/parentstyle/
---
## Style.ParentStyle property

Obtiene el estilo padre de este estilo.

```csharp
public Style ParentStyle { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyParentStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Parent Style Example";
            worksheet.Cells["A2"].Value = "Child Style Example";

            try
            {
                // Crear un estilo padre
                Style parentStyle = workbook.CreateStyle();
                parentStyle.Font.Name = "Arial";
                parentStyle.Font.Size = 12;
                parentStyle.ForegroundColor = System.Drawing.Color.LightBlue;
                parentStyle.Pattern = BackgroundType.Solid;

                // Crear un estilo hijo basado en el estilo padre
                Style childStyle = workbook.CreateStyle();
                childStyle.Font.IsBold = true;
                childStyle.Font.Color = System.Drawing.Color.Red;

                // Aplicar estilos a las celdas
                Cell parentCell = worksheet.Cells["A1"];
                parentCell.SetStyle(parentStyle);

                Cell childCell = worksheet.Cells["A2"];
                childCell.SetStyle(childStyle);

                // Demostrar la propiedad ParentStyle (solo lectura)
                Style retrievedChildStyle = childCell.GetStyle();
                Console.WriteLine("Child style has parent style: " +
                    (retrievedChildStyle.ParentStyle != null));

                if (retrievedChildStyle.ParentStyle != null)
                {
                    Console.WriteLine("Parent style font name: " +
                        retrievedChildStyle.ParentStyle.Font.Name);
                    Console.WriteLine("Parent style font size: " +
                        retrievedChildStyle.ParentStyle.Font.Size);
                }

                // Guarda el libro de trabajo
                workbook.Save("ParentStyleDemo.xlsx");
                Console.WriteLine("ParentStyle demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


