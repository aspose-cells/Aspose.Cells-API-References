---
title: "Style.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Determina se due istanze di Style sono uguali"
type: docs
url: /it/net/aspose.cells/style/equals/
---
## Style.Equals method

Determina se due istanze di Style sono uguali.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | L'oggetto Style da confrontare con l'oggetto Style corrente. |

### Valore di ritorno

true se l'Object specificato è uguale all'Object corrente; altrimenti, false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due stili da confrontare
            Style style1 = workbook.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.HorizontalAlignment = TextAlignmentType.Center;

            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Arial";
            style2.Font.Size = 12;
            style2.HorizontalAlignment = TextAlignmentType.Center;

            try
            {
                // Chiama il metodo Equals per confrontare gli stili
                bool areEqual = style1.Equals((object)style2);

                // Visualizza il risultato
                Console.WriteLine($"The styles are equal: {areEqual}");

                // Applica gli stili per dimostrare che sono identici
                if (areEqual)
                {
                    Cell cell1 = worksheet.Cells["A1"];
                    cell1.PutValue("Style 1");
                    cell1.SetStyle(style1);

                    Cell cell2 = worksheet.Cells["A2"];
                    cell2.PutValue("Style 2");
                    cell2.SetStyle(style2);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("StyleEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


