---
title: "HtmlLoadOptions.HtmlLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor HtmlLoadOptions. Crea una opción de carga del archivo"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Crea una opción de carga del archivo.

```csharp
public HtmlLoadOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Cree opciones de carga HTML usando el constructor
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;

            // Cargue el archivo HTML con las opciones
            Workbook workbook = new Workbook("example.html", loadOptions);

            // Acceda a los datos del HTML cargado
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("B1 Cell Value: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("B3 Cell Value: " + worksheet.Cells["B3"].StringValue);
            Console.WriteLine("B4 Cell Value: " + worksheet.Cells["B4"].StringValue);
        }
    }
}
```

### Ver también

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Crea una opción de carga del archivo.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadFormat | LoadFormat | El formato de carga. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Cree una instancia de HtmlLoadOptions usando el constructor con el parámetro LoadFormat
                HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);

                // Establezca algunas propiedades de HtmlLoadOptions
                loadOptions.AutoFitColsAndRows = true;
                loadOptions.SupportDivTag = true;
                loadOptions.DeleteRedundantSpaces = true;

                // Cree un libro de trabajo usando las opciones de carga
                Workbook workbook = new Workbook("input.html", loadOptions);

                // Acceder a la primera hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];

                // Mostrar alguna información sobre el HTML cargado
                Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
                Console.WriteLine($"Worksheet name: {worksheet.Name}");
                Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");

                // Guarda el libro de trabajo
                workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading HTML file: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


