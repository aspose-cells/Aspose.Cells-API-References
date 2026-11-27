---
title: "HeaderFooterCommand.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HeaderFooterCommand-egenskap. Hämtar teckensnittet för kommandots värde"
type: docs
url: /sv/net/aspose.cells/headerfootercommand/font/
---
## HeaderFooterCommand.Font property

Hämtar teckensnittet för kommandots värde.

```csharp
public Font Font { get; }
```

### Anmärkningar

Onyttig för HeaderFooterCommandType.Picture.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HeaderFooterCommandPropertyFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till sidinställningar för header/footer
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in ett header med text som kommer att ha ett HeaderFooterCommand
            pageSetup.SetHeader(0, "&\"Arial\"&12&BThis is a header");

            // Hämta header-skript
            string headerScript = pageSetup.GetHeader(0);

            // Hämta header-kommandon
            HeaderFooterCommand[] commands = pageSetup.GetCommands(headerScript);

            // Hitta textkommandot (förutsatt att det är det första)
            if (commands.Length > 0 && commands[0].Type == HeaderFooterCommandType.Text)
            {
                HeaderFooterCommand textCommand = commands[0];
                
                // Åtkomst till Font-egenskapen (skrivskyddad)
                Font font = textCommand.Font;
                
                // Visa aktuella font-egenskaper
                Console.WriteLine("Current Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");

                // Eftersom Font är skrivskyddad kan vi inte tilldela ett nytt Font-objekt,
                // men vi kan ändra befintliga font-egenskaper
                font.Name = "Times New Roman";
                font.Size = 14;
                font.IsBold = false;
                font.Color = System.Drawing.Color.Blue;

                // Spara workbook för att se ändringarna
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

### Se även

* class [Font](../../font/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


