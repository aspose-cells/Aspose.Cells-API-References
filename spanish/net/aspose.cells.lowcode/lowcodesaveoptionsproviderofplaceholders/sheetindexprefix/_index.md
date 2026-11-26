---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptionsProviderOfPlaceHolders. Prefijo para el índice de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix property

Prefijo para el índice de la hoja de cálculo.

```csharp
public string SheetIndexPrefix { get; set; }
```

### Observaciones

Si solo hay una hoja de cálculo y [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) es false, entonces este prefijo y el índice de la hoja (o nombre) no se agregarán a la ruta de archivo resultante.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexPrefixDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con múltiples hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Crear una instancia de LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheetindex}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Mostrar y modificar SheetIndexPrefix
            Console.WriteLine("Original SheetIndexPrefix: " + provider.SheetIndexPrefix);
            provider.SheetIndexPrefix = "sheet_";
            Console.WriteLine("Modified SheetIndexPrefix: " + provider.SheetIndexPrefix);

            // Establezca otras propiedades requeridas
            provider.BuildPathWithSheetAlways = true;
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();

            // Demostrar el efecto de SheetIndexPrefix en las rutas de archivo
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                // Dado que no podemos crear y poblar SplitPartInfo directamente,
                // simplemente demostraremos el patrón de nombres sin él
                Console.WriteLine($"Sheet {sheet.Name} would save to: output_{provider.SheetIndexPrefix}{sheet.Index}.xlsx");
            }

            // Guarda el libro de trabajo para demostrar el patrón de nombres
            workbook.Save("output_sheet_0.xlsx");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


