# is(selector)

- **Arguments:**
  - `{string|Component} selector`

- **Returns:** `{boolean}`

- **Usage:**

Assert every `Wrapper` in `WrapperArray` DOM node or `vm` matches [selector](/docs/en/api/selectors.md).

```js
import { mount } from 'vue-test-utils'
import { expect } from 'chai'
import Foo from './Foo.vue'

const wrapper = mount(Foo)
const divArray = wrapper.find('div')
expect(divArray.is('div')).to.equal(true)
```