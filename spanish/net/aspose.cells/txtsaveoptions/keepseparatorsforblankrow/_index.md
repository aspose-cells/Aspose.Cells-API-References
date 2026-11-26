---
title: "TxtSaveOptions.KeepSeparatorsForBlankRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Indica si los separadores deben emitirse para una fila en blanco. El valor predeterminado es false, por lo que por defecto el contenido de la fila en blanco estará vacío"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/keepseparatorsforblankrow/
---
## TxtSaveOptions.KeepSeparatorsForBlankRow property

Indica si se deben generar separadores para una fila en blanco. El valor predeterminado es falso, por lo que por defecto el contenido de la fila en blanco estará vacío.

```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyKeepSeparatorsForBlankRowDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Agregar algunos datos con filas en blanco
            cells[0, 0].PutValue("a");
            cells[0, 1].PutValue("b");
            cells[3, 0].PutValue("c");
            cells[4, 1].PutValue("d");

            // Crear opciones de guardado con KeepSeparatorsForBlankRow establecido en true
            TxtSaveOptions options = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                KeepSeparatorsForBlankRow = true
            };

            // Guarde el libro de trabajo a CSV con las opciones
            string csvOutput = SaveAsCsv(wb, options);
            Console.WriteLine(csvOutput);
        }

        private static string SaveAsCsv(Workbook wb, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                wb.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
        }
    }
}
```

### Ver también

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


