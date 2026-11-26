---
title: "PclSaveOptions.AddPrinterFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PclSaveOptions. Añade información sobre la fuente que ya está añadida a la impresora por el fabricante"
type: docs
url: /es/net/aspose.cells/pclsaveoptions/addprinterfont/
---
## PclSaveOptions.AddPrinterFont method

Agrega información sobre la fuente que ya está añadida a la impresora por el fabricante.

```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFullName | String | Nombre completo de la fuente (p. ej. "Times New Roman Bold Italic") usado en el archivo fuente. |
| fontPclName | String | Nombre de la fuente que se usará en el documento Pcl de salida. |

### Observaciones

Hay 52 fuentes que deben estar incorporadas en cualquier impresora según la especificación Pcl. Sin embargo, los fabricantes pueden añadir otras fuentes a sus dispositivos.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añade algo de texto a la hoja de cálculo para demostrar el uso de fuentes
            worksheet.Cells["A1"].PutValue("This text will use the added printer font");
            
            // Crear opciones de guardado PCL
            PclSaveOptions pclSaveOptions = new PclSaveOptions();
            
            try
            {
                // Llama al método AddPrinterFont con nombres de fuentes específicos
                pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
                pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
                
                Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
                
                // Guarda el libro de trabajo con opciones PCL
                workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


