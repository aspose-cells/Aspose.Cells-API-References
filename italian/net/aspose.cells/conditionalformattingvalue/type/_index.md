---
title: "ConditionalFormattingValue.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConditionalFormattingValue. Ottieni o imposta il tipo di questo oggetto di valore di formattazione condizionale. Impostare il tipo su FormatConditionValueType.Min o FormatConditionValueType.Max imposterà automaticamente Value a null"
type: docs
url: /it/net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

Ottieni o imposta il tipo di questo oggetto di valore di formattazione condizionale. Impostare il tipo su FormatConditionValueType.Min o FormatConditionValueType.Max imposterà automaticamente "Value" a null.

```csharp
public FormatConditionValueType Type { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValuePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet ws = workbook.Worksheets[0];

                // Aggiungi alcuni dati di esempio (necessari perché la formattazione condizionale esista)
                ws.Cells["A1"].PutValue(10);
                ws.Cells["A2"].PutValue(20);
                ws.Cells["A3"].PutValue(30);

                // Crea una raccolta di formattazione condizionale e aggiungi una condizione IconSet
                int cfIndex = ws.ConditionalFormattings.Add();
                FormatConditionCollection fcc = ws.ConditionalFormattings[cfIndex];

                int condIdx = fcc.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcc[condIdx];
                condition.IconSet.Type = IconSetType.Arrows3; // any valid icon set type

                // Ottieni un'istanza di ConditionalFormattingValue dalla raccolta IconSet
                ConditionalFormattingValue cfv = condition.IconSet.Cfvos[0];

                // Imposta il Type su Percent e assegna un valore corrispondente
                cfv.Type = FormatConditionValueType.Percent;
                cfv.Value = 25; // 25%

                // Leggi e visualizza il Type e il Value
                Console.WriteLine("After setting Type to Percent:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + cfv.Value);

                // Cambia il Type a Min – secondo la documentazione questo annullerà Value
                cfv.Type = FormatConditionValueType.Min;

                // Leggi e visualizza nuovamente il Type e il Value
                Console.WriteLine("\nAfter setting Type to Min:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + (cfv.Value == null ? "null" : cfv.Value.ToString()));

                // Salva la cartella di lavoro (la formattazione condizionale fa parte del foglio)
                workbook.Save("ConditionalFormattingValueTypeDemo.xlsx");
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

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


