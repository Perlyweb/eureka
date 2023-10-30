---
title: Bitcoin Multisig Wallet
description: Bitcoin multisig wallet setup Mermaid diagram.
toc: true
authors:
  - Satoshi
tags:
categories:
series:
date: '2023-10-30T13:11:22+08:00'
lastmod: '2023-10-30T13:11:22+08:00'
featuredImage: https://images.unsplash.com/photo-1471927866530-2b87d315d8b2?auto=format&fit=crop&q=80&w=2070&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
draft: false
---
# Bitcoin Multisig

This is a simple Mermaid dagram depicting a 2 out of 3 Bitcoin Multisig wallet.

This blog post is the first in a series where we explore multisig wallet setups in more detail. 

<div class="mermaid">
 graph LR
    A((Participant 1)) -- Public Key --> B{Bitcoin Address 1}
    A --> C((Participant 2)) 
    A --> D((Participant 3)) 
    C -- Public Key --> E{Bitcoin Address 2}
    D -- Public Key --> F{Bitcoin Address 3}
    B -- Redeem Script --> G{Multisig Address}
    E -- Redeem Script --> G
    F -- Redeem Script --> G
</div>

    