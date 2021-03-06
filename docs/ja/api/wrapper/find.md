# find(selector)

- **引数:**
  - `{string|Component} selector`

- **戻り値:** `{Wrapper}`

- **使い方:**

selectorで指定し最初のDOMノードかコンポーネントと一致した[ラッパー](/docs/ja/api/wrapper/README.md)を返します。

有効な[selector](/docs/ja/api/selectors.md)を使用してください。

```js
import { mount } from 'vue-test-utils'
import { expect } from 'chai'
import Foo from './Foo.vue'
import Bar from './Bar.vue'

const wrapper = mount(Foo)
const div = wrapper.find('div')
expect(div.is('div')).to.equal(true)
const bar = wrapper.find(Bar)
expect(bar.is(Bar)).to.equal(true)
```

- **参照:** [Wrapper](/docs/ja/api/wrapper/README.md)