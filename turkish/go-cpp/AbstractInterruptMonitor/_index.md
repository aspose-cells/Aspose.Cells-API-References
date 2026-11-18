---
title: "AbstractInterruptMonitor Sınıfı"
linktitle: "AbstractInterruptMonitor"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "AbstractInterruptMonitor sınıfı. Go'da abstractinterruptmonitor'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Tüm zaman alıcı işlemlerde kesinti isteklerini izlemek için izleme.

```go

type AbstractInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | İşlem kesintiye uğradığında, işlemi sessizce sonlandırıp sonlandırmayacağı veya bir İstisna fırlatıp fırlatmayacağı. Varsayılan false'tur, yani IsInterruptionRequested true olduğunda, ExceptionType.Interrupted kodlu bir CellsException fırlatılacaktır. |
