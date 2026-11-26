---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptionsProviderOfAssembling. Indica si siempre se agrega el índice o el nombre de la hoja a la ruta del archivo. El valor predeterminado es false, lo que significa que cuando hay solo una hoja, el índice o nombre de la hoja y el prefijo correspondiente no se agregarán a la ruta del archivo."
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways property

Indica si se agrega siempre el índice o nombre de la hoja a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una hoja, el índice (o nombre) de la hoja y el prefijo correspondiente no se agregarán a la ruta del archivo.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con una hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Crear una instancia de LowCodeSaveOptionsProviderOfAssembling
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            
            // Configurar la configuración de la ruta
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = true; // Use sheet name instead of index
            provider.SheetPrefix = "_Sheet_";
            provider.SplitPartPrefix = "_Part_";
            
            // Mostrar el valor inicial de la propiedad
            Console.WriteLine("Initial BuildPathWithSheetAlways: " + provider.BuildPathWithSheetAlways);
            
            // Demostrar la ruta del archivo sin BuildPathWithSheetAlways
            string defaultPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (default): " + defaultPath);
            
            // Establecer BuildPathWithSheetAlways en true
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine("\nAfter setting BuildPathWithSheetAlways to true: " + provider.BuildPathWithSheetAlways);
            
            // Demostrar la ruta del archivo con BuildPathWithSheetAlways (incluso con una sola hoja)
            string updatedPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (updated): " + updatedPath);
            
            // Guardar el libro de trabajo (el comportamiento de división usaría la configuración del proveedor en escenarios reales)
            workbook.Save("BuildPathWithSheetAlwaysDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


