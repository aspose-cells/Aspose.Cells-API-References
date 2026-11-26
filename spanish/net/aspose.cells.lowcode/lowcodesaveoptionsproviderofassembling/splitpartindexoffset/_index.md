---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeSaveOptionsProviderOfAssembling propiedad. Desplazamiento del índice de las partes divididas entre lo que se usa en la ruta del archivo y su valor real PartIndex"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset property

Desplazamiento del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([`PartIndex`](../../splitpartinfo/partindex/)).

```csharp
public int SplitPartIndexOffset { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartIndexOffsetDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar la hoja de cálculo para crear múltiples partes divididas
            for(int i = 0; i < 150; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Item {i+1}";
            }

            // Configurar saltos de página para dividir en 3 partes
            worksheet.HorizontalPageBreaks.Add(0, 50);
            worksheet.HorizontalPageBreaks.Add(0, 100);

            // Crear proveedor y configurar opciones de guardado
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Part_",
                SplitPartPrefix = "-",
                PathTail = ".xlsx",
                SplitPartIndexOffset = 10
            };

            // Mostrar la configuración inicial
            Console.WriteLine($"Initial SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("First save operation (offset 10):");
            Console.WriteLine($"Expected filenames: output/Part_-10.xlsx, output/Part_-11.xlsx, output/Part_-12.xlsx");

            // Cambiar el desplazamiento y mostrar la nueva configuración
            provider.SplitPartIndexOffset = 0;
            Console.WriteLine($"\nModified SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("Second save operation (offset 0):");
            Console.WriteLine($"Expected filenames: output/Part_-0.xlsx, output/Part_-1.xlsx, output/Part_-2.xlsx");

            // La operación de guardado real típicamente sería:
            // workbook.Save("output/main.xlsx", new OoxmlSaveOptions { SaveProvider = provider });
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


