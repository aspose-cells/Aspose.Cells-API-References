---
title: "FontConfigs.PreferSystemFontSubstitutes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontConfigs. Indica se utilizzare prima le sostituzioni di caratteri di sistema o meno quando un carattere non è presente e la sostituzione di questo carattere non è impostata. ad es. su Ubuntu il carattere Arial è generalmente sostituito da Liberation Sans. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/fontconfigs/prefersystemfontsubstitutes/
---
## FontConfigs.PreferSystemFontSubstitutes property

Indica se utilizzare prima le sostituzioni di caratteri di sistema o meno quando un carattere non è presente e la sostituzione di questo carattere non è impostata. Ad esempio, su Ubuntu, il carattere "Arial" è generalmente sostituito da "Liberation Sans". Il valore predefinito è false.

```csharp
public static bool PreferSystemFontSubstitutes { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyPreferSystemFontSubstitutesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Visualizza il valore corrente di PreferSystemFontSubstitutes
            Console.WriteLine("Current PreferSystemFontSubstitutes value: " + FontConfigs.PreferSystemFontSubstitutes);

            // Imposta PreferSystemFontSubstitutes su true
            FontConfigs.PreferSystemFontSubstitutes = true;
            Console.WriteLine("PreferSystemFontSubstitutes set to: " + FontConfigs.PreferSystemFontSubstitutes);

            // Crea una cella con un carattere che potrebbe richiedere una sostituzione
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with Arial font");
            Style style = cell.GetStyle();
            style.Font.Name = "Arial";
            cell.SetStyle(style);

            // Salva la cartella di lavoro per vedere gli effetti della sostituzione dei caratteri
            workbook.Save("FontSubstitutionDemo.xlsx");

            // Ripristina al valore predefinito
            FontConfigs.PreferSystemFontSubstitutes = false;
            Console.WriteLine("PreferSystemFontSubstitutes reset to: " + FontConfigs.PreferSystemFontSubstitutes);
        }
    }
}
```

### Vedi anche

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


