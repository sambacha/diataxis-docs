---
title: Developer Overview
tags:
    - Overview
    - Getting Started
---

# Documentation Overview
The document is a thorough and technical exploration of auction design and implementation in the context of Ethereum, focusing on a block proposer call market auction. It provides a detailed specification for this auction type, a glossary of terms, accounting procedures, market design considerations, and an analysis of different auction formats. The document is structured into distinct sections, each covering a critical aspect of the auction system.

## Block Proposer Call Market Auction Specification

This section serves as a technical blueprint for the proposed auction contract, detailing its properties, functions, events, storage, invariants, and testing procedures.

## Glossary 

A comprehensive glossary provides formal definitions of key terms used throughout the documentation, essential for understanding the technical language in the context of Ethereum and auction design.

## Accounting 

Discusses the financial aspects of the auction system, including various proposals for managing remunerations for validators and builders. It also introduces a bid adjustment feature for the auction system.

## Discussion Market Designs

This extensive section delves into the design considerations, updates, and trade-offs in the auction market. It covers the structure of both the primary and beta markets, along with the initial version of the MEV Protocol and auction accounting details.

## Static Sealed Bid Auctions

An analytical discussion on different auction formats, particularly focusing on uniform price and discriminatory price auctions. It proposes an augmented uniform price auction to mitigate underpricing and details the discriminatory price auction format.