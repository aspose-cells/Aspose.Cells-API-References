---
title: "Clase LowCodeSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.LowCodeSaveOptions. Opciones para guardar resultados generados de forma de bajo código"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptions/
---
## LowCodeSaveOptions class

Opciones para guardar resultados generados de forma low code.

```csharp
public class LowCodeSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Obtiene y establece el archivo (con ruta si es necesario) para guardar los datos generados. Al establecer esta propiedad con un valor distinto de null o cadena vacía, [`OutputStream`](./outputstream/) será ignorado. |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Obtiene y establece el Stream para escribir los datos generados. Al establecer esta propiedad con un valor distinto de null, [`OutputFile`](./outputfile/) será ignorado. |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | Obtiene y establece el formato de guardado para la salida. Generalmente, para procesos específicos en modo de bajo código, solo se permiten algunos formatos específicos. Por favor, especifique el formato correcto para el proceso correspondiente, de lo contrario pueden producirse resultados inesperados o incluso excepciones. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y colocar algunos datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Crear opciones de guardado
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
            {
                OutputFile = "output.xlsx"
            };

            // Guardar el libro de trabajo usando las opciones especificadas
            workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
            
            Console.WriteLine("File saved successfully with LowCodeSaveOptions");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


