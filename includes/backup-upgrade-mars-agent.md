---
title: Upgrade the Azure Backup Agent
description: This information explains why you should upgrade the Azure Backup Agent, and where to download the upgrade.
services: backup
cloud: 
suite: 
author: dcurwin
manager: carmonm

ms.service: backup
ms.tgt_pltfrm: <optional>
ms.devlang: <optional>
ms.topic: article
ms.date: 8/29/2018
ms.author: dacurwin
---

## Upgrade the MARS Agent

Versions of the Microsoft Azure Recovery Services (MARS) Agent below 2.0.9083.0 have a dependency on the Azure Access Control service. The MARS Agent is also referred to as the Azure Backup Agent.

In 2018, Microsoft [deprecated the Azure Access Control service](../articles/active-directory/azuread-dev/active-directory-acs-migration.md). Beginning March 19, 2018, all versions of the MARS Agent below 2.0.9083.0 will experience backup failures. To avoid or resolve backup failures, [upgrade your MARS Agent to the latest version](https://go.microsoft.com/fwlink/?linkid=229525). To identify servers that require a MARS Agent upgrade, follow the steps in the [Backup blog for upgrading MARS Agents](https://blogs.technet.microsoft.com/srinathv/2018/01/17/updating-azure-backup-agents/).

The MARS Agent is used to back up files and folders and system state data to Azure. System Center DPM and Azure Backup Server use the MARS Agent to back up data to Azure.
