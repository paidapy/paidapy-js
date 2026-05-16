# paidapy

Stablecoin payments for APIs and AI agents. One line of code to monetize any endpoint with the x402 protocol.

## Install

```bash
npm install @paidapy/express
```

## Usage

```typescript
import express from 'express';
import { paidapy } from '@paidapy/express';

const app = express();

app.get('/forecast',
  paidapy({ payTo: '0x...', network: 'base' }, { amount: '0.01' }),
  (req, res) => res.json({ forecast: 'sunny' })
);
```

## What is x402?

x402 is an open standard for HTTP-native payments, supported by Coinbase, Stripe, AWS, Google, Visa, and Mastercard. paidapy makes it easy to use.

## Status

Pre-alpha. Building in public.
