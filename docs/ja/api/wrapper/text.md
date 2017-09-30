# text()

- **Returns:** `{string}`

- **Usage:**

Returns text content of `Wrapper`.

```js
import { mount } from 'vue-test-utils'
import { expect } from 'chai'
import Foo from './Foo.vue'

const wrapper = mount(Foo)
expect(wrapper.text()).to.equal('bar')
```