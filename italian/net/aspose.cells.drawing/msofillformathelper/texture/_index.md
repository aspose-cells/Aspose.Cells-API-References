---
title: "MsoFillFormatHelper.Texture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormatHelper. Restituisce il tipo di riempimento texture"
type: docs
url: /it/net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

Ottiene il tipo di riempimento texture.

```csharp
public TextureType Texture { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'etichetta per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Texture Property Demo";

            try
            {
                // Crea un'istanza di MsoFillFormatHelper usando la riflessione (senza costruttore pubblico)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visualizza il valore corrente della proprietà Texture (sola lettura)
                Console.WriteLine($"Current Texture type: {fillHelper.Texture}");

                // Dimostra che la proprietà è sola lettura tentando di impostarla (commentato)
                // fillHelper.Texture = TextureType.Canvas; // Questo causerebbe un errore di compilazione

                // Mostra tutti i tipi di texture disponibili per riferimento
                Console.WriteLine("\nAvailable Texture Types:");
                foreach (TextureType textureType in Enum.GetValues(typeof(TextureType)))
                {
                    Console.WriteLine($"- {textureType}");
                }

                // Salva la cartella di lavoro per dimostrare l'esecuzione corretta
                workbook.Save("TextureDemo.xlsx");

                Console.WriteLine("\nTexture property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Texture demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


