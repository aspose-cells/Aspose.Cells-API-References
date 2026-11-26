---
title: "Clase LowCodeSaveOptionsProviderOfAssembling"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling class. Implementación para proporcionar opciones de guardado que guardan partes divididas en archivos y la ruta del archivo resultante se nombra como puede contener directorios PathHeaderSheetPrefixSheetIndexor SheetName SplitPartPrefixSplitPartIndexPathTail"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/
---
## LowCodeSaveOptionsProviderOfAssembling class

Implementación para proporcionar opciones de guardado que guardan partes divididas en archivos y la ruta del archivo resultante se nombra como (puede contener directorios): [`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex(o SheetName)+[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/).

```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | Indica si se agrega siempre el índice o nombre de la hoja a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una hoja, el índice (o nombre) de la hoja y el prefijo correspondiente no se agregarán a la ruta del archivo. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | Indica si se agrega siempre el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una parte dividida, el índice de la parte dividida y el prefijo correspondiente no se agregarán a la ruta del archivo. |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | Parte de encabezado (antes del contenido añadido de la hoja y la parte dividida) de la ruta del archivo. |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | Parte final (después de los números de secuencia) de la ruta del archivo. Debe incluir la extensión del nombre del archivo. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | La plantilla para crear una instancia de opciones de guardado en [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | Desplazamiento del índice de la hoja entre lo que se usa en la ruta del archivo y su valor real ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | Prefijo para el índice de la hoja de cálculo. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | Desplazamiento del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | Prefijo para el índice de la parte dividida. |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | Indica si se construye la ruta del archivo con el nombre de la hoja en lugar del índice de la hoja. El valor predeterminado es false. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Libera recursos después de procesar la parte dividida actual (heredado de [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;

    public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data {i + 1}";
            }

            // Inicializa y configura el proveedor de opciones de guardado
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitOutput/",
                PathTail = "_Part.xlsx",
                UseSheetName = true,
                SheetPrefix = "SHEET-",
                SplitPartPrefix = "PART-",
                BuildPathWithSheetAlways = true,
                BuildPathWithSplitPartAlways = true,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Configura las opciones de guardado XLSX con división usando LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Guarda el libro de trabajo con opciones habilitadas por el proveedor usando el formato de guardado correcto
            workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
        }
    }
}
```

### Ver también

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


