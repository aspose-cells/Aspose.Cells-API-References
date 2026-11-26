---
title: "XlsbSaveOptions.XlsbSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de XlsbSaveOptions. Crea opciones de guardado de archivo xlsb"
type: docs
url: /es/net/aspose.cells/xlsbsaveoptions/xlsbsaveoptions/
---
## XlsbSaveOptions() {#constructor}

Crea opciones de guardado de archivo xlsb.

```csharp
public XlsbSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Test Value");

            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.ExportAllColumnIndexes = true;

            workbook.Save("output.xlsb", saveOptions);
        }
    }
}
```

### Ver también

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsbSaveOptions(SaveFormat) {#constructor_1}

Crea opciones de guardado de archivo xlsb.

```csharp
[Obsolete("Use XlsbSaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public XlsbSaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de guardado. Debe ser xlsb. |

### Observaciones

NOTA: Este constructor está ahora obsoleto. En su lugar, por favor use el constructor XlsbSaveOptions(). Esta propiedad será eliminada 12 meses después desde enero de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsbSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Using XlsbSaveOptions";

            try
            {
                // Cree XlsbSaveOptions usando el constructor con el parámetro SaveFormat
                XlsbSaveOptions saveOptions = new XlsbSaveOptions(SaveFormat.Xlsb);

                // Establezca propiedades adicionales si es necesario
                saveOptions.ExportAllColumnIndexes = true;

                // Guarde el libro de trabajo con las opciones de guardado especificadas
                workbook.Save("XlsbSaveOptionsDemo.xlsb", saveOptions);

                Console.WriteLine("Workbook saved successfully with XlsbSaveOptions");
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

* enum [SaveFormat](../../saveformat/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


