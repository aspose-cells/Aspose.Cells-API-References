---
title: "AbstractTextLoadOptions.ConvertNumericData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractTextLoadOptions. Obtient ou définit une valeur qui indique si la chaîne dans le fichier texte est convertie en données numériques. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Obtient ou définit une valeur indiquant si la chaîne du fichier texte est convertie en données numériques. La valeur par défaut est true.

```csharp
public bool ConvertNumericData { get; set; }
```

### Exemples

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
            // Créez des données CSV d'exemple avec des valeurs numériques et des chaînes
            string csvData = "ID,Name,Price,Quantity\n" +
                            "1,Product A,19.99,5\n" +
                            "2,Product B,\"24.50\",\"10\"\n" +
                            "3,Product C,15.75,\"N/A\"";

            // Créez TxtLoadOptions avec ConvertNumericData défini sur true
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertNumericData = true,
                ConvertDateTimeData = true
            };

            // Chargez les données CSV dans un classeur
            Workbook workbook = new Workbook(new System.IO.MemoryStream(Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Démontrez la conversion numérique
            Console.WriteLine("Cell B2 (Product A Price) value type: " + worksheet.Cells["B2"].Value.GetType());
            Console.WriteLine("Cell B2 value: " + worksheet.Cells["B2"].Value);

            // Démontrez les valeurs de chaîne qui n'ont pas pu être converties
            Console.WriteLine("\nCell D4 (N/A) value type: " + worksheet.Cells["D4"].Value.GetType());
            Console.WriteLine("Cell D4 value: " + worksheet.Cells["D4"].Value);

            // Montrez comment les nombres entre guillemets sont toujours convertis lorsque ConvertNumericData est true
            Console.WriteLine("\nCell C3 (Quoted \"24.50\") value type: " + worksheet.Cells["C3"].Value.GetType());
            Console.WriteLine("Cell C3 value: " + worksheet.Cells["C3"].Value);
        }
    }
}
```

### Voir aussi

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


