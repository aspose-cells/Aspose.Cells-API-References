---
title: "LowCodeLoadOptions.InputFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeLoadOptions. Obtiene y establece la ruta del archivo si es necesario de la plantilla"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodeloadoptions/inputfile/
---
## LowCodeLoadOptions.InputFile property

Obtiene y establece el archivo (con ruta si es necesario) de la plantilla.

```csharp
public string InputFile { get; set; }
```

### Observaciones

Al establecer una ruta no nula y no vacía en esta propiedad, el valor previamente establecido para [`InputStream`](../inputstream/) será ignorado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeLoadOptionsPropertyInputFileDemo
    {
        public static void Run()
        {
            // Crear y guardar un archivo de plantilla de ejemplo
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
            const string templatePath = "LowCodeTemplate.xlsx";
            templateWorkbook.Save(templatePath);

            // Inicializar LowCodeLoadOptions y demostrar la propiedad InputFile
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);

            // Establecer la propiedad InputFile para usar nuestra plantilla
            loadOptions.InputFile = templatePath;
            Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);

            // Cargar el libro de trabajo usando el archivo de plantilla especificado
            Workbook workbook = new Workbook(loadOptions.InputFile);
            
            // Modificar la plantilla cargada
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);

            // Guardar el libro de trabajo modificado
            workbook.Save("PropertyInputFileDemo_Output.xlsx");
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


