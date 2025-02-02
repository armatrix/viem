# Chains

The following Viem chains are implemented on the OP Stack:

```ts
import {
  base, // [!code hl]
  baseGoerli, // [!code hl]
  baseSepolia, // [!code hl]
  optimism, // [!code hl]
  optimismGoerli, // [!code hl]
  optimismSepolia, // [!code hl]
  zora, // [!code hl]
  zoraSepolia, // [!code hl]
  zoraTestnet, // [!code hl]
} from 'viem/chains'
```

## Configuration

Viem exports OP Stack's chain [formatters](/docs/chains/formatters) & [serializers](/docs/chains/serializers) via `chainConfig`. This is useful if you need to define another chain which is implemented on the OP Stack.

```ts
import { defineChain } from 'viem'
import { chainConfig } from 'viem/op-stack'

export const opStackExample = defineChain({
  ...chainConfig,
  name: 'OP Stack Example',
  // ...
})
```
