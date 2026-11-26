---
title: "LowCodeMergeOptions.SaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeMergeOptions. Opciones de guardado para guardar las partes divididas"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodemergeoptions/saveoptions/
---
## LowCodeMergeOptions.SaveOptions property

Opciones de guardado para guardar las partes divididas.

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Merged Data");

            // Inicializar opciones de fusión
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            Console.WriteLine("Initial SaveOptions: " + (mergeOptions.SaveOptions?.GetType().Name ?? "null"));

            // Configurar nuevas opciones de guardado
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            // Establecer contraseña mediante la configuración del libro de trabajo
            workbook.Settings.Password = "Aspose1234!";
            mergeOptions.SaveOptions = saveOptions;

            // Demostrar el efecto guardando con opciones configuradas
            workbook.Save("MergedWithOptions.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Workbook saved with password-protected SaveOptions.");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


