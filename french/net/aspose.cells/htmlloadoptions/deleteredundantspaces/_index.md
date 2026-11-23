---
title: "HtmlLoadOptions.DeleteRedundantSpaces"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Indique s'il faut supprimer les espaces redondants lorsque le texte passe à la ligne en utilisant la balise br. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

Indique s'il faut supprimer les espaces redondants lorsque le texte renvoie à la ligne en utilisant la balise `<br>`. La valeur par défaut est false.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyDeleteRedundantSpacesDemo
    {
        public static void Run()
        {
            string html = "<p>   This    text   has   redundant   spaces   </p>";
            
            HtmlLoadOptions opts = new HtmlLoadOptions();
            opts.DeleteRedundantSpaces = true;
            
            byte[] htmlBytes = Encoding.UTF8.GetBytes(html);
            using (MemoryStream stream = new MemoryStream(htmlBytes))
            {
                Workbook workbook = new Workbook(stream, opts);
                Worksheet worksheet = workbook.Worksheets[0];
                
                Console.WriteLine("Cell text after removing redundant spaces: " + 
                    worksheet.Cells["A1"].StringValue);
                
                workbook.Save("output.xlsx");
            }
        }
    }
}
```

### Voir aussi

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


