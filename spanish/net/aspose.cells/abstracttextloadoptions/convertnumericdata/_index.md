---
title: "AbstractTextLoadOptions.ConvertNumericData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractTextLoadOptions. Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte a datos numéricos. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte en datos numéricos. El valor predeterminado es true.

```csharp
public bool ConvertNumericData { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Crear datos CSV de ejemplo con valores numéricos y de cadena
            string csvData = "ID,Name,Price,Quantity\n" +
                            "1,Product A,19.99,5\n" +
                            "2,Product B,\"24.50\",\"10\"\n" +
                            "3,Product C,15.75,\"N/A\"";

            // Crear TxtLoadOptions con ConvertNumericData configurado en true
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertNumericData = true,
                ConvertDateTimeData = true
            };

            // Cargue los datos CSV en un libro de trabajo
            Workbook workbook = new Workbook(new System.IO.MemoryStream(Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Demostrar la conversión numérica
            Console.WriteLine("Cell B2 (Product A Price) value type: " + worksheet.Cells["B2"].Value.GetType());
            Console.WriteLine("Cell B2 value: " + worksheet.Cells["B2"].Value);

            // Demostrar valores de cadena que no pudieron convertirse
            Console.WriteLine("\nCell D4 (N/A) value type: " + worksheet.Cells["D4"].Value.GetType());
            Console.WriteLine("Cell D4 value: " + worksheet.Cells["D4"].Value);

            // Mostrar cómo los números entre comillas aún se convierten cuando ConvertNumericData es true
            Console.WriteLine("\nCell C3 (Quoted \"24.50\") value type: " + worksheet.Cells["C3"].Value.GetType());
            Console.WriteLine("Cell C3 value: " + worksheet.Cells["C3"].Value);
        }
    }
}
```

### Ver también

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


