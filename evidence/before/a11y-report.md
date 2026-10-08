# Accessibility audit

a11y sweep @ 68eea53 dirty | 2026-10-08T04:26:48.498Z | bun 1.3.14 | FE=http://localhost:3620 BE=http://localhost:3611 gate=report

| page | passes | incomplete | critical | serious | moderate | minor |
| --- | --- | --- | --- | --- | --- | --- |
| 1. home (new thread) | 29 | 1 | 0 | 1 | 0 | 0 |
| 2. a thread | 29 | 2 | 1 | 1 | 0 | 0 |
| 3. Settings | 31 | 1 | 0 | 1 | 0 | 0 |
| 4. Bots | 26 | 2 | 0 | 0 | 0 | 0 |
| 5. Tasks | 27 | 0 | 0 | 0 | 0 | 0 |

## 1. home (new thread) - target-size (serious)

All touch targets must be 24px large, or leave sufficient space ([rule](https://dequeuniversity.com/rules/axe/4.10/target-size?application=playwright))

- ["div[aria-posinset=\"1\"] > .pr-2.pl-6.duration-150 > .rounded-md.opacity-0.transition-opacity"]

## 2. a thread - aria-required-children (critical)

Certain ARIA roles must contain particular children ([rule](https://dequeuniversity.com/rules/axe/4.10/aria-required-children?application=playwright))

- ["div[role=\"tablist\"]"]

## 2. a thread - target-size (serious)

All touch targets must be 24px large, or leave sufficient space ([rule](https://dequeuniversity.com/rules/axe/4.10/target-size?application=playwright))

- [".bg-background-secondary-hover > .rounded-md.focus-visible\\:opacity-100[title=\"Pin to Bookmarks\"]"]

## 3. Settings - target-size (serious)

All touch targets must be 24px large, or leave sufficient space ([rule](https://dequeuniversity.com/rules/axe/4.10/target-size?application=playwright))

- ["div[aria-posinset=\"1\"] > .h-8.pr-2.pl-6 > .opacity-0.transition-opacity.hover\\:bg-background-tertiary-hover"]
