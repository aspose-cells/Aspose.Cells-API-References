---
title: "SmartTagSetting.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTagSetting. Ottiene un oggetto SmartTagCollection per indice"
type: docs
url: /it/net/aspose.cells.markup/smarttagsetting/item/
---
## SmartTagSetting indexer (1 of 3)

Ottiene un oggetto [`SmartTagCollection`](../../smarttagcollection/) per indice.

```csharp
public SmartTagCollection this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| index | L'indice dell'oggetto [`SmartTagCollection`](../../smarttagcollection/) nella lista. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            
            // Dimostra l'uso della proprietà Item
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
            smartTags.Add("http://docs.aspose.com", "docs");
            
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Version", "1.0");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Vedi anche

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (2 of 3)

Ottiene l'oggetto [`SmartTagCollection`](../../smarttagcollection/) della cella.

```csharp
public SmartTagCollection this[int row, int column] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| riga | L'indice di riga della cella. |
| colonna | L'indice di colonna della cella |

### Valore di ritorno

Restituisce l'oggetto [`SmartTagCollection`](../../smarttagcollection/) della cella. Restituisce null se non ci sono tag intelligenti nella cella.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            // Dimostra l'uso della proprietà Item
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart tags in cell A1: " + smartTagCollection.Count);
            Console.WriteLine("Namespace URI: " + smartTagCollection[0].Uri);
            Console.WriteLine("Tag name: " + smartTagCollection[0].Name);

            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (3 of 3)

Ottiene l'oggetto [`SmartTagCollection`](../../smarttagcollection/) della cella.

```csharp
public SmartTagCollection this[string cellName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| cellName | Il nome della cella. |

### Valore di ritorno

Restituisce l'oggetto [`SmartTagCollection`](../../smarttagcollection/) della cella. Restituisce null se non ci sono tag intelligenti nella cella.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingPropertyItemDemo2
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Accedi a SmartTagSetting per il foglio di lavoro
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;

                // Aggiungi un tag intelligente alla cella A1 (riga 0, colonna 0)
                int smartTagIndex = smartTagSetting.Add(0, 0);

                // Dimostra l'uso della proprietà Item (indicizzatore)
                SmartTagCollection smartTagCollection = smartTagSetting[smartTagIndex];

                // Aggiungi un tag intelligente alla collezione
                smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

                // Visualizza le informazioni sul tag intelligente
                Console.WriteLine("Number of smart tags in collection: " + smartTagCollection.Count);
                if (smartTagCollection.Count > 0)
                {
                    Console.WriteLine("First smart tag URI: " + smartTagCollection[0].Uri);
                    Console.WriteLine("First smart tag name: " + smartTagCollection[0].Name);
                }

                // Salva la cartella di lavoro
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


