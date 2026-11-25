---
title: "Enum SmartTagShowType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Markup.SmartTagShowType enum. Rappresenta il tipo di visualizzazione dello smart tag"
type: docs
url: /it/net/aspose.cells.markup/smarttagshowtype/
---
## SmartTagShowType enumeration

Rappresenta il tipo di visualizzazione dello smart tag.

```csharp
public enum SmartTagShowType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| All | `0` | Indica che gli smart tag sono abilitati e mostrati |
| NoSmartTagIndicator | `1` | Indica che gli smart tag sono abilitati ma l'indicatore non viene mostrato. |
| None | `2` | Indica che gli smart tag sono disabilitati e non visualizzati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagShowTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dimostra tutti i valori dell'enum SmartTagShowType
            Console.WriteLine("SmartTagShowType values:");
            Console.WriteLine($"All: {SmartTagShowType.All}");
            Console.WriteLine($"NoSmartTagIndicator: {SmartTagShowType.NoSmartTagIndicator}");
            Console.WriteLine($"None: {SmartTagShowType.None}");

            // Crea e configura uno smart tag
            var smartTagCollection = worksheet.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");

            // Imposta le proprietà che userebbero SmartTagShowType (simulato poiché la proprietà reale non è disponibile)
            Console.WriteLine("\nSmart tag created at A1 with current date");

            // Salva con diversi scenari di tipo di visualizzazione
            workbook.Save("SmartTagShowTypeDemo_All.xlsx");
            Console.WriteLine("Workbook saved with default show type (All)");

            // Crea un altro workbook con un comportamento di tipo di visualizzazione diverso
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];
            worksheet2.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
            Console.WriteLine("\nSecond workbook created with smart tag at B2");

            workbook2.Save("SmartTagShowTypeDemo_None.xlsx");
            Console.WriteLine("Second workbook saved (simulating None behavior)");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


