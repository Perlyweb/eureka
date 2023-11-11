---
title: Bitcoin Transaction Example
description: Bitcoin Transaction setup Mermaid diagram.
toc: true
authors:
  - Satoshi
tags:
categories:
series:
date: '2023-10-30T13:11:22+08:00'
lastmod: '2023-10-30T13:11:22+08:00'
featuredImage: https://aprendizcripto.com/wp-content/uploads/2022/03/Utxo-Bitcoin.jpg
draft: false
categories: ["Bitcoin"]
tags: ["Bitcoin"]
enableComment: true
---
# Bitcoin Transaction

    participant Satoshi as Satoshi
    participant Hal as Hal
    participant Blockchain as Blockchain 

<div class="mermaid">
 sequenceDiagram
    Satoshi->Blockchain : Request to send Bitcoins
    Blockchain -->Satoshi: Transaction details and address
    Satoshi->Blockchain : Initiate transaction to Hal's address
    Blockchain -->Blockchain : Validate transaction details
    Blockchain ->Hal: Notify Hal of incoming transaction
    Hal-->Blockchain : Acknowledge receipt of transaction
    Blockchain -->Satoshi: Confirm successful transaction
</div>

    
