# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/css-parser/index.test.ts --update-snapshots` to update.

## `grid > repeat > flex`

### `ast`

```javascript
CSSRoot {
	body: [
		CSSRule {
			prelude: [
				CSSSelector {
					patterns: [
						CSSClassSelector {
							value: "style"
							loc: SourceLocation grid/repeat/flex/input.css 1:0-1:6
						}
					]
					loc: SourceLocation grid/repeat/flex/input.css 1:0-1:7
				}
			]
			block: CSSBlock {
				value: [
					CSSDeclaration {
						name: "grid-template-columns"
						value: [
							CSSRepeatFunction {
								name: "repeat"
								params: [
									CSSNumber {
										value: 4
										raw: "4"
										loc: SourceLocation grid/repeat/flex/input.css 2:31-2:32
									}
									CSSGridRepeatValue {
										values: [
											CSSDimension {
												value: 1
												unit: "fr"
												loc: SourceLocation grid/repeat/flex/input.css 2:34-2:37
											}
										]
										loc: SourceLocation grid/repeat/flex/input.css 2:34-2:37
									}
								]
								loc: SourceLocation grid/repeat/flex/input.css 2:24-2:38
							}
						]
						important: false
						loc: SourceLocation grid/repeat/flex/input.css 2:1-2:38
					}
				]
				startingTokenValue: "{"
				loc: SourceLocation grid/repeat/flex/input.css 1:7-3:1
			}
			loc: SourceLocation grid/repeat/flex/input.css 1:0-3:1
		}
	]
	comments: []
	corrupt: false
	diagnostics: []
	path: UIDPath<grid/repeat/flex/input.css>
	loc: SourceLocation grid/repeat/flex/input.css 1:0-3:1
}
```

### `diagnostics`

```

```
