---
title: "Classe SmartTagProperty"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Markup.SmartTagProperty. Rappresenta la proprietà del tag intelligente della cella"
type: docs
url: /it/net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

Rappresenta la proprietà dello smart tag della cella.

```csharp
public class SmartTagProperty
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | Ottiene e imposta il nome della proprietà. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | Ottiene e imposta il valore della proprietà. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di SmartTagProperty usando la riflessione poiché il costruttore non è pubblico
                var smartTagProperty = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Imposta le proprietà Name e Value
                smartTagProperty.Name = "DocumentType";
                smartTagProperty.Value = "FinancialReport";

                // Visualizza i valori delle proprietà
                Console.WriteLine($"SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"SmartTagProperty Value: {smartTagProperty.Value}");

                // Dimostra la modifica delle proprietà
                smartTagProperty.Name = "Status";
                smartTagProperty.Value = "Approved";

                Console.WriteLine($"Updated SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"Updated SmartTagProperty Value: {smartTagProperty.Value}");

                Console.WriteLine("SmartTagProperty demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SmartTagProperty: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


