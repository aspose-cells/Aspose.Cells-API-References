---
title: "HeaderFooterCommand.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HeaderFooterCommand. Ottiene il font del valore del comando"
type: docs
url: /it/net/aspose.cells/headerfootercommand/font/
---
## HeaderFooterCommand.Font property

Ottiene il carattere del valore del comando.

```csharp
public Font Font { get; }
```

### Osservazioni

Inutile per HeaderFooterCommandType.Picture.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HeaderFooterCommandPropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla configurazione della pagina per intestazione/piè di pagina
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta un'intestazione con testo che avrà un HeaderFooterCommand
            pageSetup.SetHeader(0, "&\"Arial\"&12&BThis is a header");

            // Ottieni lo script dell'intestazione
            string headerScript = pageSetup.GetHeader(0);

            // Ottieni i comandi di intestazione
            HeaderFooterCommand[] commands = pageSetup.GetCommands(headerScript);

            // Trova il comando di testo (presumendo sia il primo)
            if (commands.Length > 0 && commands[0].Type == HeaderFooterCommandType.Text)
            {
                HeaderFooterCommand textCommand = commands[0];
                
                // Accedi alla proprietà Font (sola lettura)
                Font font = textCommand.Font;
                
                // Visualizza le proprietà attuali del font
                Console.WriteLine("Current Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");

                // Poiché Font è di sola lettura, non possiamo assegnare un nuovo oggetto Font,
                // ma possiamo modificare le proprietà del font esistente
                font.Name = "Times New Roman";
                font.Size = 14;
                font.IsBold = false;
                font.Color = System.Drawing.Color.Blue;

                // Salva la cartella di lavoro per vedere le modifiche
                workbook.Save("HeaderFooterFontDemo.xlsx");

                Console.WriteLine("\nModified Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");
            }
        }
    }
}
```

### Vedi anche

* class [Font](../../font/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


