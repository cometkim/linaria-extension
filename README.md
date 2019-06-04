# linaria-extension

Extends Linaria usage without nesting

## Canvas

```jsx
import React from 'react'
import { css } from 'linaria'
import { ext_rule } from 'linaria-extension/macro'

const className = css`
  display: block;

  ${ext_rule(px2rem)} /* rule per line */
  font-size: 16px;
  
  ${ext_rule(provideTheme)} /* rule per block */
  & {
    color: var(--color);
    background: var(--background);
  }
`


function px2rem(property) {
  // TODO: design
}

function provideTheme(block) {
  // TODO: design
}

```
