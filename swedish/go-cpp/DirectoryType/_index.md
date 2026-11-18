---
title: "DirectoryType-enum"
linktitle: "DirectoryType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DirectoryType-enum. Inkapslar objektet som representerar directorytype i Go."
type: docs
weight: 200
url: /sv/go-cpp/directorytype/
---

## DirectoryType Enum

Representerar katalogtypen för filnamnet.

```go

type DirectoryType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [Volume](./volume/) | Representerar en MS-DOS-enhetsbokstav. Den följs av enhetsbokstaven. Eller UNC-filnamn, såsom \\server\share\myfile.xls |
| [SameVolume](./samevolume/) | Indikerar att källarboken ligger på samma enhet som den beroende arbetsboken (enhetsbokstaven utelämnas) |
| [DownDirectory](./downdirectory/) | Indikerar att källarboken ligger i en underkatalog till den aktuella katalogen. |
| [UpDirectory](./updirectory/) | Indikerar att källarboken ligger i föräldrakatalogen till den aktuella katalogen. |
