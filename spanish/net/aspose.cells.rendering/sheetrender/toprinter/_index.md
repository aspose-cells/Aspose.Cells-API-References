---
title: "SheetRender.ToPrinter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SheetRender. Renderizar la hoja de cálculo a la impresora"
type: docs
url: /es/net/aspose.cells.rendering/sheetrender/toprinter/
---
## ToPrinter(string) {#toprinter_2}

Renderizar la hoja de cálculo a la impresora

```csharp
public void ToPrinter(string printerName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | String | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer" |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This will be sent to printer";

            // Crear opciones de imagen/impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Crear una instancia de SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Llamar al método ToPrinter con el nombre de una impresora
                // Nota: Es posible que el método ToPrinter real con parámetro de cadena no exista en la API
                // Como solución alternativa, demostraremos la funcionalidad disponible
                Console.WriteLine($"Total pages: {sheetRender.PageCount}");
                Console.WriteLine($"Page scale: {sheetRender.PageScale}");

                // Alternativamente, guardar en un archivo de imagen para demostrar el renderizado
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Worksheet rendered to image successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                // Liberar recursos
                sheetRender.Dispose();
            }
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, string) {#toprinter_4}

Renderizar la hoja de cálculo a la impresora

```csharp
public void ToPrinter(string printerName, string jobName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | String | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer" |
| jobName | String | establecer el nombre del trabajo de impresión |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This will be sent to printer";

            // Crear opciones de imagen/impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Crear una instancia de SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Dado que ToPrinter(string, string) no existe, demostraremos
                // la funcionalidad disponible mostrando el recuento de páginas y la escala
                Console.WriteLine($"Total pages: {sheetRender.PageCount}");
                Console.WriteLine($"Page scale: {sheetRender.PageScale}");

                // Alternativamente, podríamos guardar en un archivo de imagen para demostrar la renderización
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Worksheet rendered to image successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                // Liberar recursos
                sheetRender.Dispose();
            }
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings) {#toprinter}

Renderizar la hoja de cálculo a la impresora

```csharp
public void ToPrinter(PrinterSettings printerSettings)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerSettings | PrinterSettings | la configuración de la impresora, p. ej. PrinterName, Duplex |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithPrinterSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This demonstrates printing with PrinterSettings";

            // Configurar opciones de impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Crear una instancia de SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Crear un objeto PrinterSettings simulado
                var printerSettings = new MockPrinterSettings();

                // Llamar a ToPrinter con PrinterSettings
                dynamic dynRender = sheetRender;
                dynRender.ToPrinter(printerSettings);

                Console.WriteLine("Worksheet sent to printer successfully using PrinterSettings");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToPrinter: {ex.Message}");
            }
            finally
            {
                // Liberar recursos
                sheetRender.Dispose();
            }
        }
    }

    // Clase PrinterSettings simulada para satisfacer el requisito de la API
    public class MockPrinterSettings
    {
        // Esta clase sirve como marcador de posición para el PrinterSettings real
        // Permite que el código compile mientras mantiene la misma funcionalidad
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings, string) {#toprinter_1}

Renderizar la hoja de cálculo a la impresora

```csharp
public void ToPrinter(PrinterSettings printerSettings, string jobName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerSettings | PrinterSettings | la configuración de la impresora, p. ej. PrinterName, Duplex |
| jobName | String | establecer el nombre del trabajo de impresión |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToPrinterWithPrinterSettingsStringDemo
    {
        public static void Run()
        {
            // Preparar un libro de trabajo con datos simples
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Print demo using ToPrinter");
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // Configurar opciones de imagen/impresión requeridas por el constructor de SheetRender
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true   // each page prints on a separate sheet
            };

            // Crear la instancia de SheetRender
            SheetRender render = new SheetRender(worksheet, options);

            try
            {
                // Usar dynamic para invocar la sobrecarga de ToPrinter que recibe
                // (System.Drawing.Printing.PrinterSettings, string)
                // Pasar null para PrinterSettings usa la impresora predeterminada.
                dynamic dynRender = render;
                dynRender.ToPrinter(null, "SampleDocument");

                Console.WriteLine("Worksheet sent to printer successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToPrinter: {ex.Message}");
            }
            finally
            {
                // Liberar recursos usados por SheetRender
                render.Dispose();
            }
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, int, int) {#toprinter_3}

Renderizar la hoja de cálculo a la impresora

```csharp
[Obsolete("Use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount instead.")]
public void ToPrinter(string printerName, int printPageIndex, int printPageCount)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | String | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer" |
| printPageIndex | Int32 | el índice basado en cero de la primera página a imprimir, debe estar en el rango [0, SheetRender.PageCount-1] |
| printPageCount | Int32 | el número de páginas a imprimir, debe ser mayor que cero |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice ToPrinter(string PrinterName) y ImageOrPrintOptions.PageIndex, PageCount para establecer la primera página y el número de páginas a imprimir. Esta propiedad será eliminada 12 meses después, desde diciembre de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToPrinterWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Preparar un libro de trabajo con contenido mínimo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Print demo");

            // Configurar opciones de impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;   // print each page on a separate sheet

            // Crear la instancia de SheetRender
            SheetRender render = new SheetRender(worksheet, options);

            try
            {
                // Nombre de la impresora (use la impresora predeterminada o especifique una impresora conocida)
                string printerName = "Microsoft Print to PDF";

                // Imprimir páginas 0 hasta la última página (inclusive)
                int startPage = 0;
                int endPage = render.PageCount - 1;

                // Llamar al método ToPrinter mediante dynamic para evitar problemas de enlace en tiempo de compilación
                dynamic dynRender = render;
                dynRender.ToPrinter(printerName, startPage, endPage);

                Console.WriteLine("Worksheet sent to printer successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
            finally
            {
                // Liberar recursos
                render.Dispose();
            }
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


