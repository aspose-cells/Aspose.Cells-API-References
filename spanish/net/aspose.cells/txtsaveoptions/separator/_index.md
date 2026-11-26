---
title: "TxtSaveOptions.Separator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Obtiene y establece el delimitador de carácter del archivo de texto"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/separator/
---
## TxtSaveOptions.Separator property

Obtiene y establece el carácter delimitador del archivo de texto.

```csharp
public char Separator { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Configure las opciones de guardado TXT con separador de coma
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.Separator = ',';
            txtSaveOptions.Encoding = System.Text.Encoding.UTF8;

            // Guarde el libro de trabajo como CSV con separador de coma
            string outputPath = "output.csv";
            workbook.Save(outputPath, txtSaveOptions);

            // Muestre el contenido del archivo guardado
            Console.WriteLine("File saved with comma separator:");
            Console.WriteLine(File.ReadAllText(outputPath));
        }
    }
}
```

### Ver también

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


