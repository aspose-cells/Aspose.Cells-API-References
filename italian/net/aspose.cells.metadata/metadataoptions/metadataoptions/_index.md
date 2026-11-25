---
title: "MetadataOptions.MetadataOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MetadataOptions costruttore. Crea un'opzione per il caricamento dei metadati"
type: docs
url: /it/net/aspose.cells.metadata/metadataoptions/metadataoptions/
---
## MetadataOptions constructor

Crea un'opzione per il caricamento dei metadati.

```csharp
public MetadataOptions(MetadataType metadataType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| metadataType | MetadataType | Il tipo di metadati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsMethodCtorWithMetadataTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Chiama il metodo #ctor con il parametro MetadataType
                MetadataOptions options = new MetadataOptions(MetadataType.Encryption);
                
                // Imposta proprietà aggiuntive
                options.Password = "test123";
                options.KeyLength = 128;
                
                // Visualizza le opzioni create
                Console.WriteLine($"MetadataType: {options.MetadataType}");
                Console.WriteLine($"Password set: {!string.IsNullOrEmpty(options.Password)}");
                Console.WriteLine($"KeyLength: {options.KeyLength}");

                // Usa le opzioni durante il caricamento dei metadati (esempio)
                // Questo verrebbe tipicamente usato con LoadOptions durante l'apertura di un file
                // Nota: Il codice originale ha provato a impostare MetadataOptions direttamente su LoadOptions,
                // ma la classe LoadOptions non ha questa proprietà nella definizione fornita.
                // Terremo solo la parte di creazione delle opzioni poiché l'utilizzo con LoadOptions
                // non è possibile con la definizione API corrente.
                
                Console.WriteLine("MetadataOptions created successfully with MetadataType parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating MetadataOptions: {ex.Message}");
            }
            
            // Salva la cartella di lavoro (anche se le opzioni dei metadati non influirebbero su questa cartella di lavoro vuota)
            workbook.Save("MetadataOptionsCtorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


