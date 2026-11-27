---
title: "WorkbookMetadata.Save"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookMetadata‑metod. Spara den modifierade metadata till filen"
type: docs
url: /sv/net/aspose.cells.metadata/workbookmetadata/save/
---
## Save(string) {#save_1}

Spara den modifierade metadata till filen.

```csharp
public void Save(string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Filnamnet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Skapa ny metadata för arbetsbok
            WorkbookMetadata doc = new WorkbookMetadata("example.xlsb", new MetadataOptions(Aspose.Cells.Metadata.MetadataType.DocumentProperties));
            
            // Lägg till anpassade egenskaper
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            
            // Spara med strängsökväg
            doc.Save("output.xlsb");
            
            // Verifiera den sparade filen
            Workbook workbook = new Workbook("output.xlsb");
            Console.WriteLine("File saved successfully with custom properties.");
            Console.WriteLine("Property 'text1' value: " + doc.CustomDocumentProperties["text1"].Value.ToString());
        }
    }
}
```

### Se även

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream) {#save}

Spara den modifierade metadata till strömmen.

```csharp
public void Save(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Strömmen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.IO;
    using Aspose.Cells;
    using Aspose.Cells.Metadata;

    public class WorkbookMetadataMethodSaveWithStreamDemo
    {
        public static void Run()
        {
            try
            {
                // Sökväg till en befintlig arbetsbok (se till att filen finns i körmappen)
                string sourcePath = "Sample.xlsx";

                // Skapa MetadataOptions för dokumentegenskaper
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Instansiera WorkbookMetadata med källfilen och alternativen
                WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);

                // Åtkomst till den inbyggda samlingen av dokumentegenskaper (skrivskyddad)
                var builtInProperties = metadata.BuiltInDocumentProperties;
                Console.WriteLine("Built‑in document properties collection retrieved.");

                // Spara metadata till en ny fil med en ström
                using (FileStream outputStream = new FileStream("MetadataOutput.xlsx",
                                                              FileMode.Create,
                                                              FileAccess.Write))
                {
                    metadata.Save(outputStream);
                }

                Console.WriteLine("Metadata saved successfully to stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during metadata Save: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


