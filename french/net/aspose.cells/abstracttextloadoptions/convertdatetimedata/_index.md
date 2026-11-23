---
title: "AbstractTextLoadOptions.ConvertDateTimeData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractTextLoadOptions. Obtient ou définit une valeur indiquant si la chaîne du fichier texte est convertie en données de date. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Obtient ou définit une valeur indiquant si la chaîne du fichier texte est convertie en données de date. La valeur par défaut est true.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertDateTimeDataDemo
    {
        public static void Run()
        {
            // Créer des données CSV avec une chaîne de date
            string csvData = "\"2023-05-15\",\"123.45\"";

            // Créer des options de chargement de texte avec ConvertDateTimeData défini sur false
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            options.ConvertDateTimeData = false;
            options.ConvertNumericData = false;

            // Charger les données CSV
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Afficher les valeurs (devraient rester sous forme de chaînes)
            Console.WriteLine("Cell A1 value: " + worksheet.Cells[0, 0].StringValue); // Outputs "2023-05-15" as string
            Console.WriteLine("Cell B1 value: " + worksheet.Cells[0, 1].StringValue); // Outputs "123.45" as string

            // Chargez maintenant avec ConvertDateTimeData défini sur true
            options.ConvertDateTimeData = true;
            options.ConvertNumericData = true;
            workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            worksheet = workbook.Worksheets[0];

            // Affichez les valeurs converties
            Console.WriteLine("Cell A1 value (converted): " + worksheet.Cells[0, 0].DateTimeValue); // Outputs DateTime
            Console.WriteLine("Cell B1 value (converted): " + worksheet.Cells[0, 1].DoubleValue);  // Outputs 123.45 as double
        }
    }
}
```

### Voir aussi

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


