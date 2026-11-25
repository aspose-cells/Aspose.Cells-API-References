---
title: "OoxmlSaveOptions.AsFlatOpc"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OoxmlSaveOptions. Indica se salvare come file flat opc che può essere generato da Open XML SDK"
type: docs
url: /it/net/aspose.cells/ooxmlsaveoptions/asflatopc/
---
## OoxmlSaveOptions.AsFlatOpc property

Indica se salvare come file OPC piatto che può essere generato dall'Open XML SDK.

```csharp
public bool AsFlatOpc { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Flat OPC Demo");

            try
            {
                // Crea un'istanza di OoxmlSaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Visualizza il valore predefinito della proprietà AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Imposta AsFlatOpc su true
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Salva la cartella di lavoro con AsFlatOpc abilitato
                workbook.Save("AsFlatOpc_Enabled.xlsx", saveOptions);

                // Crea un'altra opzione di salvataggio con AsFlatOpc disabilitato
                OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
                saveOptions2.AsFlatOpc = false;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions2.AsFlatOpc);

                // Salva la cartella di lavoro con AsFlatOpc disabilitato
                workbook.Save("AsFlatOpc_Disabled.xlsx", saveOptions2);

                Console.WriteLine("AsFlatOpc property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


