---
title: "TxtLoadOptions.TreatQuotePrefixAsValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es verdadero. Si es falso, la comilla simple inicial se eliminará del valor de la celda correspondiente y QuotePrefix se establecerá como verdadero para la celda."
type: docs
url: /es/net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es verdadero. Si es falso, la comilla simple inicial se eliminará del valor de la celda correspondiente y [`QuotePrefix`](../../style/quoteprefix/) se establecerá como verdadero para la celda.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTreatQuotePrefixAsValueDemo
    {
        public static void Run()
        {
            // Crear datos CSV de ejemplo con prefijos de comillas
            string csvData = "ID,Name,Value\n1,\"'Apple\",100\n2,\"'Orange\",200";
            string filePath = "test.csv";

            // Guardar los datos CSV en un archivo
            File.WriteAllText(filePath, csvData);

            // Escenario 1: TreatQuotePrefixAsValue = false (por defecto)
            var loadOptions1 = new TxtLoadOptions();
            loadOptions1.TreatQuotePrefixAsValue = false;
            
            var workbook1 = new Workbook(filePath, loadOptions1);
            var worksheet1 = workbook1.Worksheets[0];
            Console.WriteLine("TreatQuotePrefixAsValue = false:");
            Console.WriteLine("Cell B2 value: " + worksheet1.Cells["B2"].Value); // Will show 'Apple (quote treated as formatting)

            // Escenario 2: TreatQuotePrefixAsValue = true
            var loadOptions2 = new TxtLoadOptions();
            loadOptions2.TreatQuotePrefixAsValue = true;
            
            var workbook2 = new Workbook(filePath, loadOptions2);
            var worksheet2 = workbook2.Worksheets[0];
            Console.WriteLine("\nTreatQuotePrefixAsValue = true:");
            Console.WriteLine("Cell B2 value: " + worksheet2.Cells["B2"].Value); // Will show 'Apple (quote treated as value)

            // Limpiar
            File.Delete(filePath);
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


