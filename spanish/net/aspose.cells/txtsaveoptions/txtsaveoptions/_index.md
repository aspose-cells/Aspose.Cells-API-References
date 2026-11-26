---
title: "TxtSaveOptions.TxtSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de TxtSaveOptions. Crea opciones de guardado de archivo de texto"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/txtsaveoptions/
---
## TxtSaveOptions() {#constructor}

Crea opciones de guardado de archivo de texto.

```csharp
public TxtSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Demostrar el constructor de TxtSaveOptions
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.SeparatorString = "|";
            
            // Guarda con separador personalizado
            workbook.Save("output.txt", txtSaveOptions);
            
            Console.WriteLine("File saved with custom separator successfully.");
        }
    }
}
```

### Ver también

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtSaveOptions(SaveFormat) {#constructor_1}

Crea opciones de guardado de archivo de texto.

```csharp
public TxtSaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de archivo. Debe ser Csv o Tsv, de lo contrario el formato guardado se establecerá como Csv automáticamente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class TxtSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Llamar al método #ctor con el parámetro SaveFormat
                TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
                
                // Configura las opciones de guardado
                saveOptions.Separator = ',';
                saveOptions.Encoding = Encoding.UTF8;
                saveOptions.QuoteType = TxtValueQuoteType.Always;
                
                Console.WriteLine("TxtSaveOptions created successfully with SaveFormat.Csv");
                
                // Guarda el libro de trabajo con las opciones configuradas
                workbook.Save("TxtSaveOptionsDemo.csv", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing TxtSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


