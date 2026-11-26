---
title: "OoxmlSaveOptions.OoxmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor OoxmlSaveOptions. Crea las opciones para guardar un archivo Office Open XML"
type: docs
url: /es/net/aspose.cells/ooxmlsaveoptions/ooxmlsaveoptions/
---
## OoxmlSaveOptions() {#constructor}

Crea las opciones para guardar el archivo Office Open XML.

```csharp
public OoxmlSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo y agregar algunos datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Demostrar el constructor OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            
            // Guardar el libro con opciones OOXML
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML options.");
        }
    }
}
```

### Ver también

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OoxmlSaveOptions(SaveFormat) {#constructor_1}

Crea las opciones para guardar el archivo Office Open XML.

```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de archivo. Debe ser uno de los siguientes tipos: Xlsx, Xltx, Xlam, Xlsm o Xltm, de lo contrario el formato guardado se establecerá automáticamente como Xlsx. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            try
            {
                // Crear OoxmlSaveOptions con el parámetro SaveFormat
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                
                // Establecer algunas propiedades de las opciones de guardado
                saveOptions.ExportCellName = true;
                saveOptions.CompressionType = OoxmlCompressionType.Level6;
                
                Console.WriteLine("OoxmlSaveOptions created successfully with SaveFormat.Xlsx");
                
                // Guardar el libro de trabajo con las opciones especificadas
                workbook.Save("OoxmlSaveOptionsCtorDemo.xlsx", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating OoxmlSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


