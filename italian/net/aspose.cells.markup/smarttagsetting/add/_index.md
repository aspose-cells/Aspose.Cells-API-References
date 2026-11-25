---
title: "SmartTagSetting.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SmartTagSetting. Aggiunge un oggetto SmartTagCollection a una cella"
type: docs
url: /it/net/aspose.cells.markup/smarttagsetting/add/
---
## Add(int, int) {#add}

Aggiunge un oggetto [`SmartTagCollection`](../../smarttagcollection/) a una cella.

```csharp
public int Add(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | La riga della cella. |
| colonna | Int32 | La colonna della cella. |

### Valore di ritorno

Restituisce l'indice di un oggetto [`SmartTagCollection`](../../smarttagcollection/) nel foglio di lavoro.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Add to cell A1 (row 0, column 0)

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());
            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Aggiungi smart tag a una cella.

```csharp
public int Add(string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Il nome della cella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni l'istanza SmartTagSetting
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            
            try
            {
                // Chiama il metodo Add con parametro String
                int index = smartTagSetting.Add("A1");
                
                Console.WriteLine($"SmartTag added successfully at index: {index}");
                
                // Aggiungi del contenuto per dimostrare l'effetto
                worksheet.Cells["A1"].PutValue("This cell has a smart tag");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("SmartTagSettingMethodAddWithStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


