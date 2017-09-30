# hasClass(className)

- **Arguments:**
  - `{string} className`

- **Returns:** `{boolean}`

- **Usage:**

Assert every `Wrapper` in `WrapperArray` DOM node has class containing `className`. 

```js
import { mount } from 'vue-test-utils'
import { expect } from 'chai'
import Foo from './Foo.vue'

const wrapper = mount(Foo)
const divArray = wrapper.findAll('div')
expect(divArray.hasClass('bar')).to.equal(true)
```
