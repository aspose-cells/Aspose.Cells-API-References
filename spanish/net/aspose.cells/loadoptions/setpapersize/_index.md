---
title: "LoadOptions.SetPaperSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LoadOptions. Establece el tamaño de papel de impresión predeterminado a partir de la configuración de impresoras predeterminadas"
type: docs
url: /es/net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

Establece el tamaño de papel de impresión predeterminado a partir de la configuración de la impresora predeterminada.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | PaperSizeType | El tamaño de papel predeterminado. |

### Observaciones

Si no hay una configuración sobre el tamaño de papel, MS Excel usará la configuración predeterminada de la impresora.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsMethodSetPaperSizeWithPaperSizeTypeDemo
    {
        public static void Run()
        {
            // Crear LoadOptions y establecer el tamaño de papel a A5
            LoadOptions options = new LoadOptions();
            options.SetPaperSize(PaperSizeType.PaperA5);

            // Cargar el libro de trabajo con las opciones especificadas
            Workbook workbook = new Workbook("example.xlsx", options);
            
            // Verificar que el tamaño de papel esté configurado correctamente
            Console.WriteLine("Paper size of first worksheet: " + workbook.Worksheets[0].PageSetup.PaperSize);
        }
    }
}
```

### Ver también

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


