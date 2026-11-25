---
title: "DefaultStyleSettings.FontName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DefaultStyleSettings. Ottiene/Imposta il nome del carattere predefinito per la cartella di lavoro"
type: docs
url: /it/net/aspose.cells/defaultstylesettings/fontname/
---
## DefaultStyleSettings.FontName property

Ottiene/Imposta il nome del carattere predefinito per la cartella di lavoro

```csharp
public string FontName { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontNameDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento e imposta il nome del carattere
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.FontName = "SimSun";

            // Crea una nuova cartella di lavoro con le opzioni di caricamento
            Workbook workbook = new Workbook();
            workbook.DefaultStyle.Font.Name = loadOptions.DefaultStyleSettings.FontName;

            // Accedi allo stile predefinito e verifica il nome del carattere
            Style defaultStyle = workbook.DefaultStyle;
            Console.WriteLine("Default Font Name: " + defaultStyle.Font.Name);

            // Crea un foglio di lavoro e imposta il valore della cella
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Name Test");

            // Salva la cartella di lavoro
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Console.WriteLine("Workbook saved with default font: SimSun");
            }
        }
    }
}
```

### Vedi anche

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


