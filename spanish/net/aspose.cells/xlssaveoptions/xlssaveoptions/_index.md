---
title: "XlsSaveOptions.XlsSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de XlsSaveOptions. Crea opciones para guardar un archivo Excel 972003 xls"
type: docs
url: /es/net/aspose.cells/xlssaveoptions/xlssaveoptions/
---
## XlsSaveOptions() {#constructor}

Crea opciones para guardar el archivo Excel 97-2003 xls.

```csharp
public XlsSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Sample XLS File");
            worksheet.Cells["A2"].PutValue("Created using XlsSaveOptions");

            // Inicializar XlsSaveOptions usando el constructor
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            // Establecer algunas opciones (propiedades no compatibles eliminadas)
            saveOptions.IsTemplate = false;

            // Guardar el libro de trabajo con las opciones
            workbook.Save("output.xls", saveOptions);

            Console.WriteLine("File saved successfully with XlsSaveOptions.");
        }
    }
}
```

### Ver también

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsSaveOptions(SaveFormat) {#constructor_1}

Crea opciones para guardar el archivo Excel 97-2003 xls/xlt.

```csharp
public XlsSaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato del archivo. Debe ser Excel97To2003 o Xlt, de lo contrario el formato guardado se establecerá automáticamente como Excel97To2003. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);
            
            try
            {
                // Llamar al método #ctor con el parámetro SaveFormat
                XlsSaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Excel97To2003);
                
                // Establecer propiedades adicionales
                saveOptions.MatchColor = true;
                saveOptions.WpsCompatibility = false;
                
                Console.WriteLine("XlsSaveOptions constructor executed successfully with SaveFormat parameter");
                
                // Guardar el libro de trabajo con las opciones especificadas
                workbook.Save("XlsSaveOptionsCtorDemo.xls", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XlsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


