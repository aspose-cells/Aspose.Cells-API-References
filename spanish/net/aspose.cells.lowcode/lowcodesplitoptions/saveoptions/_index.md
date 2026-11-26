---
title: "LowCodeSplitOptions.SaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSplitOptions. Opciones de guardado para guardar las partes divididas"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptions/
---
## LowCodeSplitOptions.SaveOptions property

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

    public class LowCodeSplitOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y agregar datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Crea una instancia de LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Mostrar valor inicial de SaveOptions (null por defecto)
            Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));

            // Crear y configurar LowCodeSaveOptions para formato PDF
            LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
            pdfSaveOptions.SaveFormat = SaveFormat.Pdf;

            // Asignar las opciones de guardado a SplitOptions
            splitOptions.SaveOptions = pdfSaveOptions;

            // Mostrar valor actualizado de SaveOptions
            Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);

            // Escenario de uso de ejemplo: Dividir el libro de trabajo guardaría las partes como PDF
            // (El código real de división dependería de la implementación de la API Aspose.Cells.LowCode)
            // LowCodeEngine.Split(workbook, splitOptions, "output_directory/");
            
            // Guarda el libro de trabajo original para demostración (no afectado por SplitOptions)
            workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


