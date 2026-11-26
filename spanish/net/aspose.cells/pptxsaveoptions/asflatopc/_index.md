---
title: "PptxSaveOptions.AsFlatOpc"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PptxSaveOptions. Indica si se guarda como un archivo OPC plano que puede ser generado por Open XML SDK"
type: docs
url: /es/net/aspose.cells/pptxsaveoptions/asflatopc/
---
## PptxSaveOptions.AsFlatOpc property

Indica si se guarda como un archivo opc plano que puede ser generado por Open XML SDK

```csharp
public bool AsFlatOpc { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PptxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Flat OPC Demo";

            try
            {
                // Crear una instancia de PptxSaveOptions
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Mostrar el valor predeterminado de AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Establecer la propiedad a true para demostrar su uso
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Guardar el libro de trabajo como PPTX con la opción habilitada
                workbook.Save("AsFlatOpcDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with AsFlatOpc enabled");
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

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


