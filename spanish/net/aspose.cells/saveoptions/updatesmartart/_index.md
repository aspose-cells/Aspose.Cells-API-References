---
title: "SaveOptions.UpdateSmartArt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Indica si se actualiza la configuración de SmartArt. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/saveoptions/updatesmartart/
---
## SaveOptions.UpdateSmartArt property

Indica si se actualiza la configuración de SmartArt. El valor predeterminado es false.

```csharp
public bool UpdateSmartArt { get; set; }
```

### Observaciones

Solo tiene efecto después de llamar al método Shape.GetResultOfSmartArt() y que las formas en caché existan en el archivo de plantilla.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyUpdateSmartArtDemo
    {
        public static void Run()
        {
            // Cargar el libro de trabajo de origen
            Workbook workbook = new Workbook("example.xlsx");

            // Modificar formas y SmartArt
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    shape.AlternativeText = "ReplacedAlternativeText";
                    
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            smartArtShape.Text = "ReplacedText";
                        }
                    }
                }
            }

            // Guardar con UpdateSmartArt habilitado
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.UpdateSmartArt = true;
            workbook.Save("output.xlsx", saveOptions);

            // Verificar los cambios
            Workbook savedWorkbook = new Workbook("output.xlsx");
            foreach (Worksheet worksheet in savedWorkbook.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    Console.WriteLine($"Shape Alt Text: {shape.AlternativeText}");
                    
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            Console.WriteLine($"SmartArt Text: {smartArtShape.Text}");
                        }
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


