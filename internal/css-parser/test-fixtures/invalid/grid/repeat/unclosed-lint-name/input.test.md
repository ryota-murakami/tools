# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/css-parser/index.test.ts --update-snapshots` to update.

## `invalid > grid > repeat > unclosed-lint-name`

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
							loc: SourceLocation invalid/grid/repeat/unclosed-lint-name/input.css 1:0-1:6
						}
					]
					loc: SourceLocation invalid/grid/repeat/unclosed-lint-name/input.css 1:0-1:7
				}
			]
			block: CSSBlock {
				value: [
					CSSDeclaration {
						name: "grid-template-columns"
						value: [
							CSSFunction {
								name: "repeat"
								params: []
								loc: SourceLocation invalid/grid/repeat/unclosed-lint-name/input.css 2:24-2:44
							}
							CSSRaw {
								loc: SourceLocation invalid/grid/repeat/unclosed-lint-name/input.css 2:44-2:45
							}
						]
						important: false
						loc: SourceLocation invalid/grid/repeat/unclosed-lint-name/input.css 2:1-2:45
					}
				]
				startingTokenValue: "{"
				loc: SourceLocation invalid/grid/repeat/unclosed-lint-name/input.css 1:7-3:1
			}
			loc: SourceLocation invalid/grid/repeat/unclosed-lint-name/input.css 1:0-3:1
		}
	]
	comments: []
	corrupt: false
	diagnostics: [
		{
			origins: [{entity: "ParserCore<css>"}]
			description: {
				advice: [
					log {category: "info", text: [RAW_MARKUP {value: "Add a <emphasis>]</emphasis> after <emphasis>"}, "col-start", RAW_MARKUP {value: "</emphasis>."}]}
				]
				category: ["parse"]
				categoryValue: "css"
				message: RAW_MARKUP {value: "The line name doesn't have a closing square bracket"}
			}
			location: {
				language: "css"
				path: UIDPath<invalid/grid/repeat/unclosed-lint-name/input.css>
				end: Position 2:35
				start: Position 2:34
			}
		}
	]
	path: UIDPath<invalid/grid/repeat/unclosed-lint-name/input.css>
	loc: SourceLocation invalid/grid/repeat/unclosed-lint-name/input.css 1:0-3:1
}
```

### `diagnostics`

```

 invalid/grid/repeat/unclosed-lint-name/input.css:2:34 parse(css) ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ The line name doesn't have a closing square bracket

    1 │ .style {
  > 2 │   grid-template-columns: repeat(4, [col-start);
      │                                    ^
    3 │ }

  ℹ Add a ] after col-start.


```
