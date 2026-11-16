---
title: "SystemTimeInterruptMonitor Class"
linktitle: "SystemTimeInterruptMonitor"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "SystemTimeInterruptMonitor class. Encapsule l'objet qui représente systemtimeinterruptmonitor en Go."
type: docs
weight: 200
url: /fr/go-cpp/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Implémentation simple de <see cref=\"AbstractInterruptMonitor\"/> en vérifiant et en comparant l'heure système actuelle avec la limite spécifiée par l'utilisateur.

```go

type SystemTimeInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewSystemTimeInterruptMonitor](./newsystemtimeinterruptmonitor/) | Construit un moniteur d'interruption. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [StartMonitor](./startmonitor/) | Démarre le moniteur avec la limite de temps spécifiée. Le moment de départ pour calculer le coût en temps est exactement le moment où cette méthode est appelée, donc la procédure qui doit être surveillée doit être lancée immédiatement après cet appel. |
| [IsInterruptionRequested](./isinterruptionrequested/) | Cette implémentation vérifie simplement si le coût en temps (du moment où le moniteur démarre jusqu'à maintenant) est supérieur à la limite spécifiée par l'utilisateur. |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | Voir AbstractInterruptMonitor.TerminateWithoutException. Cette propriété est spécifiée par l'utilisateur lors de la construction de cette instance de moniteur. |
