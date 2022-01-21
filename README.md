# nextjs-lazy-load
Showcase: Lazy load component with Next.js 12 & React 18

[Next.js: React 18 Installation](https://nextjs.org/docs/advanced-features/react-18)

```
import dynamic from "next/dynamic";
import {Suspense} from 'react'
...
const LazyLoadComponent = dynamic<{}>(() => import('../components/lazy-load-component'), {
    suspense: true,
})
...
<Suspense fallback={`loading`}>
    <LazyLoadComponent/>
</Suspense>
```
