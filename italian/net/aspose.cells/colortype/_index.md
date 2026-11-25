---
title: "Enum ColorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ColorType enum. Rappresenta tutti i tipi di colore"
type: docs
url: /it/net/aspose.cells/colortype/
---
## ColorType enumeration

Rappresenta tutti i tipi di colore

```csharp
public enum ColorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Colore automatico. |
| AutomaticIndex | `1` | È colore automatico, ma il colore visualizzato dipende dall'impostazione del sistema operativo. |
| RGB | `2` | Il colore RGB. |
| IndexedColor | `3` | L'indice di colore nella tavolozza dei colori. |
| Theme | `4` | Il colore del tema. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassColorTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook per la dimostrazione
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Dimostrare l'uso dei valori dell'enumerazione ColorType
                ColorType automatic = ColorType.Automatic;
                ColorType rgb = ColorType.RGB;
                ColorType theme = ColorType.Theme;

                // Visualizzare i valori dell'enumerazione
                Console.WriteLine($"Automatic color type value: {(int)automatic}");
                Console.WriteLine($"RGB color type value: {(int)rgb}");
                Console.WriteLine($"Theme color type value: {(int)theme}");

                // Creare una cella e impostarne il valore
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ColorType Demo");

                // Creare uno stile e applicarlo alla cella
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Black;
                cell.SetStyle(style);

                // Salva la cartella di lavoro
                workbook.Save("ColorTypeDemo.xlsx");

                Console.WriteLine("ColorType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ColorType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


