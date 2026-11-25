---
title: "Worksheet.CustomProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà del foglio di lavoro. Ottiene un oggetto che rappresenta le informazioni identificative associate a un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Ottiene un oggetto che rappresenta le informazioni di identificatore associate a un foglio di lavoro.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Osservazioni

Worksheet.CustomProperties fornisce un meccanismo preferito per memorizzare dati arbitrari. Supporta componenti di documenti di terze parti legacy, così come quelle situazioni che hanno un'esigenza stringente di parti binarie.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCustomPropertiesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi proprietà personalizzate al foglio di lavoro
            worksheet.CustomProperties.Add("Property1", "Value1");
            worksheet.CustomProperties.Add("Property2", "12345");
            worksheet.CustomProperties.Add("Property3", DateTime.Now.ToString());
            
            // Visualizza il conteggio delle proprietà personalizzate
            Console.WriteLine("Custom Properties Count: " + worksheet.CustomProperties.Count);
            
            // Accedi e visualizza i valori delle proprietà
            foreach (var prop in worksheet.CustomProperties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetCustomPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


