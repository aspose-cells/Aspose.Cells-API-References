---
title: "Enum TxtValueQuoteType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.TxtValueQuoteType. Especifica el tipo de uso de comillas para valores en archivos de formato de texto."
type: docs
url: /es/net/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enumeration

Especifica el tipo de uso de comillas para los valores en archivos de formato de texto.

```csharp
public enum TxtValueQuoteType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Normal | `0` | Todos los valores que contengan caracteres especiales como comillas o carácter separador serán entrecomillados. Igual que el comportamiento de MS Excel al exportar archivos de texto. |
| Always | `1` | Todos los valores siempre estarán entrecomillados. |
| Minimum | `2` | Solo entrecomillar los valores cuando sea necesario. Por ejemplo, si un valor contiene comillas pero la comilla no está al inicio de ese valor, ese valor no será entrecomillado. |
| Never | `3` | Ningún valor será entrecomillado. El archivo de texto exportado con este tipo puede no leerse correctamente porque faltan las comillas necesarias. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtValueQuoteTypeDemo
    {
        public static void TxtValueQuoteTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells[0, 0].Value = "Name";
            worksheet.Cells[0, 1].Value = "Age";
            worksheet.Cells[1, 0].Value = "John Doe";
            worksheet.Cells[1, 1].Value = 30;
            worksheet.Cells[2, 0].Value = "Jane Smith";
            worksheet.Cells[2, 1].Value = 25;

            // Crear TxtSaveOptions y establecer el QuoteType
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.QuoteType = TxtValueQuoteType.Always;

            // Guardar el libro de trabajo como un archivo de texto con el tipo de comillas especificado
            workbook.Save("TxtValueQuoteTypeExample.txt", saveOptions);

            Console.WriteLine("Workbook saved with TxtValueQuoteType.Always");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


