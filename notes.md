## what next optimizes
1. Optimizes fonts, when used by next/font module. It downloads font files at build time and hosts them with your other static assets. This means there are no additional network requests for fonts which would impact performance.

2. Next can server static assets like images, from public folder. We should use the <Image> component, that comes with automatic image optimizations, such as, lazy loading, prevent layout shift, resize images, use modern formats when possible

3. Using those, the cumulative layout shift is improved.

4. Layout doesn't re-render but only page, on navigation
5. automatic code-splitting and prefetching, when use <Link> component from next/link. Entire app is not loaded at once, the pages become isolated, one page shown error, it doesn't migrate to other pages.
6. <Link> lead to automatic prefetching, whenever a link comes in the viewport, to improve user exp.

## Features in next
1. navigate using next/link, page won't refresh
    Active links are shown using usePathname() hook.
2. images using next/images
3. fonts from next/font
4.