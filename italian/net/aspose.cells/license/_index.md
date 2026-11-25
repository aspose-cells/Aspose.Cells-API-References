---
title: "Classe License"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.License. Fornisce metodi per licenziare il componente"
type: docs
url: /it/net/aspose.cells/license/
---
## License class

Fornisce metodi per licenziare il componente.

```csharp
public class License
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [License](license/)() | Inizializza una nuova istanza di questa classe. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense)(Stream) | Licenzia il componente. |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense_1)(string) | Licenzia il componente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LicenseDemo
    {
        public static void LicenseExample()
        {
            // Crea un'istanza della classe License
            License license = new License();

            // Imposta la licenza utilizzando il nome di un file di licenza
            license.SetLicense("Aspose.Cells.NET.lic");

            // In alternativa, imposta la licenza utilizzando uno stream
            using (FileStream licenseStream = new FileStream("Aspose.Cells.NET.lic", FileMode.Open))
            {
                license.SetLicense(licenseStream);
            }

            // Codice aggiuntivo per dimostrare l'utilizzo della funzionalità licenziata di Aspose.Cells
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            // Salva la cartella di lavoro per verificare che la licenza sia applicata correttamente
            workbook.Save("LicensedWorkbook.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


