# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `es2015 > uncategorised > 128`

### `ast`

```javascript
JSRoot {
	body: [
		JSClassDeclaration {
			id: JSBindingIdentifier {
				name: "A"
				loc: SourceLocation es2015/uncategorised/128/input.js 1:6-1:7 (A)
			}
			meta: JSClassHead {
				body: [
					JSClassMethod {
						kind: "method"
						key: JSStaticPropertyKey {
							value: JSIdentifier {
								name: "foo"
								loc: SourceLocation es2015/uncategorised/128/input.js 1:16-1:19 (foo)
							}
							loc: SourceLocation es2015/uncategorised/128/input.js 1:16-1:19
						}
						meta: JSClassPropertyMeta {
							abstract: false
							declare: false
							optional: false
							readonly: false
							static: true
							loc: SourceLocation es2015/uncategorised/128/input.js 1:9-1:19
							start: Position 1:9
						}
						body: JSBlockStatement {
							body: []
							directives: []
							loc: SourceLocation es2015/uncategorised/128/input.js 1:22-1:24
						}
						head: JSFunctionHead {
							async: false
							generator: false
							hasHoistedVars: false
							params: []
							loc: SourceLocation es2015/uncategorised/128/input.js 1:19-1:21
						}
						loc: SourceLocation es2015/uncategorised/128/input.js 1:9-1:24
					}
				]
				loc: SourceLocation es2015/uncategorised/128/input.js 1:0-1:25
			}
			loc: SourceLocation es2015/uncategorised/128/input.js 1:0-1:25
		}
	]
	comments: []
	corrupt: false
	diagnostics: []
	directives: []
	hasHoistedVars: false
	sourceType: "script"
	syntax: []
	path: UIDPath<es2015/uncategorised/128/input.js>
	loc: SourceLocation es2015/uncategorised/128/input.js 1:0-1:25
}
```

### `diagnostics`

```

```
