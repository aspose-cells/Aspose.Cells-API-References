---
title: "Workbook.AddDigitalSignature"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Aggiunge una firma digitale a un file di foglio di calcolo OOXML Excel2007 e versioni successive"
type: docs
url: /it/net/aspose.cells/workbook/adddigitalsignature/
---
## Workbook.AddDigitalSignature method

Aggiunge la firma digitale a un file di foglio di calcolo OOXML (Excel2007 e versioni successive).

```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Osservazioni

Supporta solo l'aggiunta di firma digitale Xmldsig a un file di foglio di calcolo OOXML

### Esempi

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAddDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati di esempio
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature");

            // Carica certificato (sostituisci con il percorso del tuo certificato e la password)
            X509Certificate2 certificate = new X509Certificate2("DrWatson.pfx", "1234567890");

            // Crea firma digitale
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);

            // Crea una collezione di firme digitali e aggiungi la firma
            DigitalSignatureCollection digitalSignatureCollection = new DigitalSignatureCollection();
            digitalSignatureCollection.Add(digitalSignature);

            // Aggiungi firma digitale al workbook
            workbook.AddDigitalSignature(digitalSignatureCollection);

            // Salva la cartella di lavoro
            workbook.Save("DigitallySignedWorkbook.xlsx");
        }
    }
}
```

### Vedi anche

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


