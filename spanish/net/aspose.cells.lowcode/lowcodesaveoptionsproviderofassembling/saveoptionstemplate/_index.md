---
title: "LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeSaveOptionsProviderOfAssembling propiedad. La plantilla para crear una instancia de opciones de guardado en GetSaveOptions"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate property

La plantilla para crear una instancia de opciones de guardado en [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Observaciones

Si la plantilla ha sido especificada, entonces la instancia creada copiará todas las configuraciones de ella y actualizará el archivo de salida en consecuencia.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con dos hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet worksheet1 = workbook.Worksheets[0];
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet1.Cells["A1"].PutValue("Sheet1 Content");
            worksheet2.Cells["A1"].PutValue("Sheet2 Content");

            // Crear una instancia de LowCodeSaveOptionsProviderOfAssembling
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "Output/Sheet",
                PathTail = ".xlsx",
                BuildPathWithSheetAlways = true,
                UseSheetName = false
            };

            // Mostrar el estado inicial de SaveOptionsTemplate
            Console.WriteLine("Initial SaveOptionsTemplate is " + (provider.SaveOptionsTemplate == null ? "null" : "set"));

            // Configurar SaveOptionsTemplate con cifrado
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();
            Console.WriteLine("SaveOptionsTemplate configured");

            // Crear opciones de guardado LowCode
            var saveOptions = new LowCodeSaveOptions();

            // Guardar el libro de trabajo usando el proveedor configurado (generará archivos separados por hoja)
            workbook.Save("output_combined.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Demo executed successfully. Check output files.");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


