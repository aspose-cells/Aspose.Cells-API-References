---
title: "HtmlSaveOptions.EnableCssCustomProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottimizza l'output dell'html utilizzando le proprietà CSS personalizzate. Ad esempio, nello scenario in cui ci sono più occorrenze di un'immagine base64 con proprietà personalizzata, i dati dell'immagine devono essere salvati una sola volta, così le prestazioni dell'html risultante possono essere migliorate. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/enablecsscustomproperties/
---
## HtmlSaveOptions.EnableCssCustomProperties property

Ottimizza l'output dell'html utilizzando le proprietà personalizzate CSS. Ad esempio, nello scenario in cui ci sono più occorrenze di una stessa immagine base64, con una proprietà personalizzata i dati dell'immagine devono essere salvati una sola volta, migliorando così le prestazioni dell'html risultante. Il valore predefinito è false.

```csharp
public bool EnableCssCustomProperties { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con formattazione
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;

            // Aggiungi un'immagine che verrà ripetuta in più celle
            int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
            Picture pic = worksheet.Pictures[imgIndex];
            pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
            pic.Width = 100;
            pic.Height = 100;

            // Copia l'immagine in un'altra posizione
            worksheet.Cells["D5"].PutValue("Same image reference:");
            int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
            pic2.Width = 100;
            pic2.Height = 100;

            // Crea un'istanza di HtmlSaveOptions
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

            // Visualizza il valore corrente
            Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);

            // Imposta su true per ottimizzare l'output CSS
            htmlOptions.EnableCssCustomProperties = true;

            // Salva con ottimizzazione CSS
            workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);

            // Imposta su false per il confronto
            htmlOptions.EnableCssCustomProperties = false;
            workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);

            Console.WriteLine("Files saved with and without CSS custom properties optimization.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


