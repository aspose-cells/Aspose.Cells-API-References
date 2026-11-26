---
title: "PclSaveOptions.PclSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de PclSaveOptions. Crea las opciones para guardar un archivo pcl"
type: docs
url: /es/net/aspose.cells/pclsaveoptions/pclsaveoptions/
---
## PclSaveOptions constructor

Crea las opciones para guardar un archivo pcl.

```csharp
public PclSaveOptions()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
            
            try
            {
                // Llama al método #ctor para crear una instancia de PclSaveOptions
                PclSaveOptions pclOptions = new PclSaveOptions();
                
                // Configura opciones adicionales si es necesario
                pclOptions.AddPrinterFont("Arial", "ArialPCL");
                
                Console.WriteLine("PclSaveOptions created successfully");
                
                // Guarda el libro de trabajo con opciones PCL
                workbook.Save("PclSaveOptionsDemo.pcl", pclOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating PclSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


