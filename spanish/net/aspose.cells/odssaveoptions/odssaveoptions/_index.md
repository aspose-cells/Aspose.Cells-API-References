---
title: "OdsSaveOptions.OdsSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor OdsSaveOptions. Crea las opciones para guardar el archivo ods"
type: docs
url: /es/net/aspose.cells/odssaveoptions/odssaveoptions/
---
## OdsSaveOptions() {#constructor}

Crea las opciones de guardado del archivo ods.

```csharp
public OdsSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar celdas de ejemplo con diferentes estilos de borde
            worksheet.Cells["B2"].PutValue("Medium Border");
            worksheet.Cells["B4"].PutValue("Thick Border");
            worksheet.Cells["B7"].PutValue("Double Border");
            
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Medium;
            worksheet.Cells["B2"].SetStyle(style);
            
            style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            worksheet.Cells["B4"].SetStyle(style);
            
            style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            worksheet.Cells["B7"].SetStyle(style);

            // Demostrar el constructor OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
            
            // Guardar como archivo ODS
            workbook.Save("output.ods", saveOptions);
            
            Console.WriteLine("File saved with OdsSaveOptions constructor demo.");
        }
    }
}
```

### Ver también

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsSaveOptions(SaveFormat) {#constructor_1}

Crea las opciones de guardado del archivo ods.

```csharp
public OdsSaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de archivo. Debe ser Ods, Ots, Fods o Sxc, de lo contrario el formato guardado se establecerá automáticamente como Ods. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsSaveOptionsMethodCtorWithSaveFormatDemo
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
                OdsSaveOptions saveOptions = new OdsSaveOptions(SaveFormat.Ods);
                
                // Establecer algunas propiedades de las opciones de guardado
                saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
                saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
                
                Console.WriteLine("OdsSaveOptions constructor executed successfully with SaveFormat.Ods parameter");
                
                // Guardar el libro de trabajo con las opciones especificadas
                workbook.Save("OdsSaveOptionsCtorDemo.ods", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OdsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


