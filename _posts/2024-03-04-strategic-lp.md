---
title: Strategic LP in UniV3
description: Strategic Liquidity Provision in Uniswap V3
author: 1e-18
date: 2024-06-25 11:33:00 +0800
categories: [concentrated liquidity, strategy]
tags: [clmm, amm, lp]
pin: true
math: true
mermaid: true
image:
  path: https://www.researchgate.net/publication/353863135/figure/fig1/AS:1056191211909120@1628827016954/Illustration-for-the-reserve-curve-for-Uniswap-v2-v3-When-the-liquidity-is.ppm
  lqip: data:image/webp;base64,UklGRpoAAABXRUJQVlA4WAoAAAAQAAAADwAABwAAQUxQSDIAAAARL0AmbZurmr57yyIiqE8oiG0bejIYEQTgqiDA9vqnsUSI6H+oAERp2HZ65qP/VIAWAFZQOCBCAAAA8AEAnQEqEAAIAAVAfCWkAALp8sF8rgRgAP7o9FDvMCkMde9PK7euH5M1m6VWoDXf2FkP3BqV0ZYbO6NA/VFIAAAA
  alt: https://www.researchgate.net/figure/Illustration-for-the-reserve-curve-for-Uniswap-v2-v3-When-the-liquidity-is_fig1_353863135
---


Review notes on “Strategic Liquidity Provision in Uniswap V3” [2021]

[Strategic Liquidity Provision in Uniswap v3](https://arxiv.org/pdf/2106.12033v4)

> “We formalize the dynamic liquidity provision problem, and focus on a general class of strategies for which we provide a neural network-based optimization framework for maximizing LP earnings. We model a single LP that faces an exogenous sequence of price changes that arise from arbitrage and non-arbitrage trades in the decentralized exchange.”
* Fan et al (2021)*
> 

# Introduction

## The contributions of this paper are as follows:

- Reset-LP strategies
    - Uniform
    - Proportional
    - Optimal
- Expected utility of a reset-LP strategy
- Optimal reset-LP strategy based on price change statistics from historical price data
- Demonstrating that proportional allocations are optimal for risk-seeking providers and uniform allocations are optimal for risk-averse providers
- Back-testing an optimal reset-LP strategy to demonstrate that under suitable conditions, a strategic provider will earn 200x more return vs v2 strategy