# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `es2015 > uncategorised > 347`

### `ast`

```javascript
JSRoot {
	body: [
		JSClassDeclaration {
			id: JSBindingIdentifier {
				name: "A"
				loc: SourceLocation es2015/uncategorised/347/input.js 1:6-1:7 (A)
			}
			meta: JSClassHead {
				body: [
					JSClassMethod {
						kind: "set"
						key: JSStaticPropertyKey {
							value: JSIdentifier {
								name: "prop"
								loc: SourceLocation es2015/uncategorised/347/input.js 1:14-1:18 (prop)
							}
							loc: SourceLocation es2015/uncategorised/347/input.js 1:14-1:18
						}
						meta: JSClassPropertyMeta {
							abstract: false
							declare: false
							optional: false
							readonly: false
							static: false
							loc: SourceLocation es2015/uncategorised/347/input.js 1:10-1:18
							start: Position 1:10
						}
						body: JSBlockStatement {
							body: []
							directives: []
							loc: SourceLocation es2015/uncategorised/347/input.js 1:25-1:27
						}
						head: JSFunctionHead {
							async: false
							generator: false
							hasHoistedVars: false
							params: [
								JSBindingIdentifier {
									name: "x"
									meta: JSPatternMeta {
										loc: SourceLocation es2015/uncategorised/347/input.js 1:19-1:20
									}
									loc: SourceLocation es2015/uncategorised/347/input.js 1:19-1:20 (x)
								}
								JSBindingIdentifier {
									name: "y"
									meta: JSPatternMeta {
										loc: SourceLocation es2015/uncategorised/347/input.js 1:22-1:23
									}
									loc: SourceLocation es2015/uncategorised/347/input.js 1:22-1:23 (y)
								}
							]
							loc: SourceLocation es2015/uncategorised/347/input.js 1:18-1:24
						}
						loc: SourceLocation es2015/uncategorised/347/input.js 1:10-1:27
					}
				]
				loc: SourceLocation es2015/uncategorised/347/input.js 1:0-1:29
			}
			loc: SourceLocation es2015/uncategorised/347/input.js 1:0-1:29
		}
	]
	comments: []
	corrupt: false
	diagnostics: [
		{
			origins: [{entity: "ParserCore<js>"}]
			description: {
				advice: []
				category: ["parse"]
				categoryValue: "js"
				message: RAW_MARKUP {value: "setter should have exactly one param"}
			}
			location: {
				language: "js"
				path: UIDPath<es2015/uncategorised/347/input.js>
				end: Position 1:27
				start: Position 1:10
			}
		}
	]
	directives: []
	hasHoistedVars: false
	sourceType: "script"
	syntax: []
	path: UIDPath<es2015/uncategorised/347/input.js>
	loc: SourceLocation es2015/uncategorised/347/input.js 1:0-1:29
}
```

### `diagnostics`

```

 es2015/uncategorised/347/input.js:1:10 parse(js) ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ setter should have exactly one param

    class A { set prop(x, y) {} }
              ^^^^^^^^^^^^^^^^^


```
