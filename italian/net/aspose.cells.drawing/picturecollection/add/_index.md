---
title: Add
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Aggiunge unimmagine alla raccolta.
type: docs
weight: 20
url: /it/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Aggiunge un'immagine alla raccolta.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftRow | Int32 | Indice della riga in alto a sinistra. |
| upperLeftColumn | Int32 | Indice della colonna in alto a sinistra. |
| lowerRightRow | Int32 | Indice della riga in basso a destra |
| lowerRightColumn | Int32 | Indice della colonna in basso a destra |
| stream | Stream | Oggetto stream che contiene i dati dell'immagine. |

### Valore di ritorno

[`Picture`](../../picture) indice oggetto.

### Esempi

```csharp

[C#]
//aggiungi una foto
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, 5, 5, fs);
}
```

### Guarda anche

* class [PictureCollection](../../picturecollection)
* spazio dei nomi [Aspose.Cells.Drawing](../../picturecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Aggiunge un'immagine alla raccolta.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftRow | Int32 | Indice della riga in alto a sinistra. |
| upperLeftColumn | Int32 | Indice della colonna in alto a sinistra. |
| lowerRightRow | Int32 | Indice della riga in basso a destra |
| lowerRightColumn | Int32 | Indice della colonna in basso a destra |
| fileName | String | Nome file immagine. |

### Valore di ritorno

[`Picture`](../../picture) indice oggetto.

### Esempi

```csharp

[C#]
//aggiungi una foto
pictures.Add(1, 1, 5, 5, "image.jpg");
```

### Guarda anche

* class [PictureCollection](../../picturecollection)
* spazio dei nomi [Aspose.Cells.Drawing](../../picturecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Aggiunge un'immagine alla raccolta.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftRow | Int32 | Indice della riga in alto a sinistra. |
| upperLeftColumn | Int32 | Indice della colonna in alto a sinistra. |
| stream | Stream | Oggetto stream che contiene i dati dell'immagine. |

### Valore di ritorno

[`Picture`](../../picture) indice oggetto.

### Esempi

```csharp

[C#]
//aggiungi una foto
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs);
}
```

### Guarda anche

* class [PictureCollection](../../picturecollection)
* spazio dei nomi [Aspose.Cells.Drawing](../../picturecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Aggiunge un'immagine alla raccolta.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftRow | Int32 | Indice della riga in alto a sinistra. |
| upperLeftColumn | Int32 | Indice della colonna in alto a sinistra. |
| fileName | String | Nome file immagine. |

### Valore di ritorno

[`Picture`](../../picture) indice oggetto.

### Esempi

```csharp

[C#]
//aggiungi una foto
pictures.Add(1, 1, "image.jpg");
```

### Guarda anche

* class [PictureCollection](../../picturecollection)
* spazio dei nomi [Aspose.Cells.Drawing](../../picturecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Aggiunge un'immagine alla raccolta.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftRow | Int32 | Indice della riga in alto a sinistra. |
| upperLeftColumn | Int32 | Indice della colonna in alto a sinistra. |
| stream | Stream | Oggetto stream che contiene i dati dell'immagine. |
| widthScale | Int32 | Scala della larghezza dell'immagine, una percentuale. |
| heightScale | Int32 | Scala dell'altezza dell'immagine, una percentuale. |

### Valore di ritorno

[`Picture`](../../picture) indice oggetto.

### Esempi

```csharp

[C#]
//aggiungi una foto
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Guarda anche

* class [PictureCollection](../../picturecollection)
* spazio dei nomi [Aspose.Cells.Drawing](../../picturecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Aggiunge un'immagine alla raccolta.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale, 
    int heightScale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftRow | Int32 | Indice della riga in alto a sinistra. |
| upperLeftColumn | Int32 | Indice della colonna in alto a sinistra. |
| fileName | String | Nome file immagine. |
| widthScale | Int32 | Scala della larghezza dell'immagine, una percentuale. |
| heightScale | Int32 | Scala dell'altezza dell'immagine, una percentuale. |

### Valore di ritorno

[`Picture`](../../picture) indice oggetto.

### Esempi

```csharp

[C#]
//aggiungi una foto
pictures.Add(1, 1, "image.jpg", 50, 50);
```

### Guarda anche

* class [PictureCollection](../../picturecollection)
* spazio dei nomi [Aspose.Cells.Drawing](../../picturecollection)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
