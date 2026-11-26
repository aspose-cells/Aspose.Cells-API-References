---
title: "PageSetup.FitToPagesTall"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el número de páginas de alto al que se escalará la hoja de cálculo cuando se imprima. El valor predeterminado es 1"
type: docs
url: /es/net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

Representa el número de páginas de altura a las que se escalará la hoja de cálculo cuando se imprima. El valor predeterminado es 1.

```csharp
public int FitToPagesTall { get; set; }
```

### Observaciones

Debe establecer FitToPagesWide en cero si desea ajustar todas las filas en una sola página.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesTallDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para que la hoja abarque varias páginas
            for (int i = 0; i < 100; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            // Obtener el objeto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establecer área de impresión
            pageSetup.PrintArea = "A1:J100";
            
            // Establecer la propiedad FitToPagesTall para que todas las filas quepan en una página
            pageSetup.FitToPagesTall = 1;
            
            // Establecer la propiedad FitToPagesWide para que todas las columnas quepan en una página
            pageSetup.FitToPagesWide = 1;
            
            // Establecer el tamaño del papel
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Imprimir líneas de cuadrícula
            pageSetup.PrintGridlines = true;

            // Crear opciones de renderizado
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Crear renderizador de hoja
            SheetRender render = new SheetRender(worksheet, options);
            
            // Mostrar la escala de la página
            Console.WriteLine($"Page scale: {Math.Round(render.PageScale, 2)}");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


