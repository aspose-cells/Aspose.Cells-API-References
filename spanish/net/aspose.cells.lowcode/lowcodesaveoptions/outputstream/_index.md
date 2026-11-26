---
title: "LowCodeSaveOptions.OutputStream"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptions. Obtiene y establece el Stream para escribir los datos generados. Al establecer esta propiedad con un valor distinto de null, OutputFile será ignorado"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptions/outputstream/
---
## LowCodeSaveOptions.OutputStream property

Obtiene y establece el Stream para escribir los datos generados. Al establecer esta propiedad con un valor distinto de null, [`OutputFile`](../outputfile/) será ignorado.

```csharp
public Stream OutputStream { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class LowCodeSaveOptionsPropertyOutputStreamDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");

            try
            {
                // Crear instancia de LowCodeSaveOptions
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                
                // Crear un flujo de memoria para demostración
                using (MemoryStream stream = new MemoryStream())
                {
                    // Establecer la propiedad OutputStream
                    saveOptions.OutputStream = stream;
                    saveOptions.SaveFormat = SaveFormat.Xlsx;

                    // Guardar usando las opciones (escribirá en nuestro flujo de memoria)
                    workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);

                    // Verificar que el flujo fue escrito
                    Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
                    Console.WriteLine("OutputStream position reset to 0 for reading");
                    saveOptions.OutputStream.Position = 0;

                    // Crear un nuevo libro de trabajo a partir del flujo para verificar el contenido
                    Workbook verifyWorkbook = new Workbook(saveOptions.OutputStream);
                    Console.WriteLine($"Verified worksheet count: {verifyWorkbook.Worksheets.Count}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


