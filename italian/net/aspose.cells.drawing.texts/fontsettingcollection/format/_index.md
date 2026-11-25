---
title: "FontSettingCollection.Format"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontSettingCollection. Formatta il testo con le impostazioni del font"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/format/
---
## FontSettingCollection.Format method

Formatta il testo con l'impostazione del font.

```csharp
public void Format(int startIndex, int length, Font font, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | Int32 | L'indice di partenza. |
| lunghezza | Int32 | La lunghezza. |
| font | Font | Il font. |
| flag | StyleFlag | Le flag del font. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodFormatWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Imposta il testo iniziale
            fontSettingCollection.Text = "Sample Text for Formatting";

            try
            {
                // Crea uno stile e imposta le sue proprietà del font
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                style.Font.IsBold = true;
                style.Font.Color = System.Drawing.Color.Red;

                // Crea un flag di stile per specificare quali proprietà del font applicare
                StyleFlag styleFlag = new StyleFlag();
                styleFlag.FontName = true;
                styleFlag.FontSize = true;
                styleFlag.FontBold = true;
                styleFlag.FontColor = true;

                // Formatta i caratteri dall'indice 7 all'11 (la parola "Text")
                fontSettingCollection.Format(7, 4, style.Font, styleFlag);

                // Salva la cartella di lavoro per mostrare l'effetto
                workbook.Save("FontSettingCollectionFormatDemo.xlsx");
                Console.WriteLine("Format method executed successfully. Text 'Text' is now bold, red Arial 14pt.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


