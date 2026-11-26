---
title: "Clase LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders. Implementación para proporcionar opciones de guardado que guardan partes divididas en archivos y la ruta del archivo resultante se define con marcadores de posición"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders class

Implementación para proporcionar opciones de guardado que guardan las partes divididas en archivos y la ruta del archivo resultante se define con marcadores de posición.

```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | Instancia un objeto para proporcionar opciones de guardado según plantillas especificadas. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | Indica si siempre se agrega el índice o nombre de la hoja a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una hoja, el índice y nombre de la hoja y el prefijo correspondiente([`SheetNamePrefix`](./sheetnameprefix/)) no se agregarán a la ruta del archivo. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | Indica si siempre se agrega el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una parte dividida, el índice de la parte y el prefijo correspondiente([`SplitPartPrefix`](./splitpartprefix/)) no se agregarán a la ruta del archivo. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | La plantilla para crear una instancia de opciones de guardado en [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | Desplazamiento del índice de la hoja entre lo que se usa en la ruta del archivo y su valor real ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | Prefijo para el índice de la hoja de cálculo. |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | Prefijo para el índice de la hoja de cálculo. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | Desplazamiento del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | Prefijo para el índice de la parte dividida. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Libera recursos después de procesar la parte dividida actual (heredado de [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;

    public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar la hoja de cálculo con datos de ejemplo
            for (int i = 0; i < 250; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Crear proveedor con plantilla de ruta que contiene marcadores de posición
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
            
            // Configurar propiedades del proveedor
            provider.SheetIndexOffset = 1;
            provider.SplitPartIndexOffset = 1;
            provider.SheetIndexPrefix = "S";
            provider.SplitPartPrefix = "P";
            provider.BuildPathWithSheetAlways = true;
            provider.BuildPathWithSplitPartAlways = true;

            // Configurar plantilla de opciones de guardado
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Configurar opciones de imagen o impresión para el renderizado dividido
            var imgOrPrintOptions = new ImageOrPrintOptions
            {
                SaveFormat = SaveFormat.Pdf,
                OnePagePerSheet = false,
                PageIndex = 0,
                PageCount = 1
            };

            // Crear renderizado de hoja con configuración de división
            var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
            sheetRender.ToImage(0, "output"); // This would normally split and save using provider
        }
    }
}
```

### Ver también

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


