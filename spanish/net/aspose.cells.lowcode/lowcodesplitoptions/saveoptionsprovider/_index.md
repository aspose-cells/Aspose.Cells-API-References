---
title: "LowCodeSplitOptions.SaveOptionsProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSplitOptions. Proveedor de opciones de guardado para guardar las partes divididas"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/
---
## LowCodeSplitOptions.SaveOptionsProvider property

Proveedor de opciones de guardado para guardar las partes divididas.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Observaciones

Si se especifica esta propiedad, [`SaveOptions`](../saveoptions/) no tiene efecto porque la salida de cada parte dividida será especificada por el proveedor.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Crear instancia de LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Mostrar valor actual de SaveOptionsProvider (null por defecto)
            Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Crear un SaveOptionsProvider personalizado
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Demostrar el efecto de establecer SaveOptionsProvider
            // En un escenario real, esto se usaría al dividir archivos
            Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Guardar el libro de trabajo (aunque la división no se muestra aquí)
            workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
        }
    }

    // Implementación personalizada de AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Crear opciones de guardado personalizadas para cada parte dividida
            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            return options;
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Realizar cualquier limpieza después de guardar cada parte
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Ver también

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


