---
title: "OoxmlSaveOptions.AsFlatOpc"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OoxmlSaveOptions. Indica si se guarda como un archivo flat opc que puede ser generado por Open XML SDK"
type: docs
url: /es/net/aspose.cells/ooxmlsaveoptions/asflatopc/
---
## OoxmlSaveOptions.AsFlatOpc property

Indica si se guarda como un archivo OPC plano que puede ser generado por el SDK de Open XML.

```csharp
public bool AsFlatOpc { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Flat OPC Demo");

            try
            {
                // Crear una instancia de OoxmlSaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Muestre el valor predeterminado de la propiedad AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Establecer AsFlatOpc a true
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Guardar el libro con AsFlatOpc habilitado
                workbook.Save("AsFlatOpc_Enabled.xlsx", saveOptions);

                // Crear otra opción de guardado con AsFlatOpc deshabilitado
                OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
                saveOptions2.AsFlatOpc = false;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions2.AsFlatOpc);

                // Guardar el libro con AsFlatOpc deshabilitado
                workbook.Save("AsFlatOpc_Disabled.xlsx", saveOptions2);

                Console.WriteLine("AsFlatOpc property demonstration completed successfully.");
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

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


