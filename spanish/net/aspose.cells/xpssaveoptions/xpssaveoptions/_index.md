---
title: "XpsSaveOptions.XpsSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor XpsSaveOptions. Crea opciones para guardar un archivo xps"
type: docs
url: /es/net/aspose.cells/xpssaveoptions/xpssaveoptions/
---
## XpsSaveOptions() {#constructor}

Crea opciones para guardar el archivo xps.

```csharp
public XpsSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XpsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("XPS Save Options Demo");

            // Inicializar XpsSaveOptions usando el constructor
            XpsSaveOptions saveOptions = new XpsSaveOptions();

            // Configurar opciones de guardado
            saveOptions.OnePagePerSheet = true;
            saveOptions.DefaultFont = "Arial";
            saveOptions.PageIndex = 0;
            saveOptions.PageCount = 1;

            // Guardar el libro de trabajo con opciones
            workbook.Save("XpsSaveOptionsDemo.xps", saveOptions);
        }
    }
}
```

### Ver también

* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XpsSaveOptions(SaveFormat) {#constructor_1}

Crea opciones para guardar el archivo xps.

```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de guardado, debe ser formato xps. |

### Observaciones

NOTA: Este constructor está ahora obsoleto. En su lugar, utilice el constructor XpsSaveOptions(). Esta propiedad será eliminada 12 meses después desde agosto de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XpsSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "XPS Save Options Demo";
            worksheet.Cells["B1"].Value = "Using SaveFormat parameter";

            try
            {
                // Cree XpsSaveOptions usando el constructor con el parámetro SaveFormat
                XpsSaveOptions saveOptions = new XpsSaveOptions(SaveFormat.Xps);

                // Guardar el libro de trabajo con las opciones especificadas
                workbook.Save("XpsSaveOptionsWithSaveFormatDemo.xps", saveOptions);

                Console.WriteLine("XpsSaveOptions created successfully with SaveFormat parameter");
                Console.WriteLine("Workbook saved as XPS format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating XpsSaveOptions or saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


