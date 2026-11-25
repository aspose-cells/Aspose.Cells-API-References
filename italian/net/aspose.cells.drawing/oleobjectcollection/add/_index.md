---
title: "OleObjectCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo OleObjectCollection. Aggiunge un OleObject alla collezione"
type: docs
url: /it/net/aspose.cells.drawing/oleobjectcollection/add/
---
## Add(int, int, int, int, byte[]) {#add}

Aggiunge un OleObject alla collezione.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| altezza | Int32 | Altezza dell'oleObject, in unità di pixel. |
| larghezza | Int32 | Larghezza dell'oleObject, in unità di pixel. |
| imageData | Byte[] | Immagine dell'ole object come array di byte. |

### Valore di ritorno

[`OleObject`](../../oleobject/) object index.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati dell'oggetto OLE (file Excel di esempio come array di byte)
            byte[] oleData;
            try
            {
                string sampleFilePath = "sample.xlsx";
                oleData = File.ReadAllBytes(sampleFilePath);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error reading sample file: {ex.Message}");
                return;
            }

            try
            {
                // Chiama il metodo Add con i parametri: (upperLeftRow, upperLeftColumn, height, width, imageData)
                int oleIndex = worksheet.OleObjects.Add(5, 2, 200, 300, oleData);

                Console.WriteLine($"OLE object added successfully at index: {oleIndex}");
                Console.WriteLine($"Position: Row 5, Column 2");
                Console.WriteLine($"Size: 200px height, 300px width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, byte[], string) {#add_1}

Aggiunge un OleObject collegato alla collezione.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData, 
    string linkedFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| altezza | Int32 | Altezza dell'oleObject, in unità di pixel. |
| larghezza | Int32 | Larghezza dell'oleObject, in unità di pixel. |
| imageData | Byte[] | Immagine dell'ole object come array di byte. |
| linkedFile | String |  |

### Valore di ritorno

[`OleObject`](../../oleobject/) object index.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati dell'oggetto OLE
            int upperLeftRow = 1;
            int upperLeftColumn = 1;
            int height = 200;
            int width = 200;
            byte[] imageData = File.ReadAllBytes("sample.ole");
            string linkedFile = "sample.xlsx";

            try
            {
                // Chiama il metodo Add con i tipi di parametro specifici
                int index = worksheet.OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData, linkedFile);
                
                Console.WriteLine($"OLE object added at index: {index}");
                Console.WriteLine($"Total OLE objects in worksheet: {worksheet.OleObjects.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


