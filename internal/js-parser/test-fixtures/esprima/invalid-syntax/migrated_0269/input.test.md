# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `esprima > invalid-syntax > migrated_0269`

### `ast`

```javascript
JSRoot {
	body: [
		JSClassDeclaration {
			id: JSBindingIdentifier {
				name: "A"
				loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:6-1:7 (A)
			}
			meta: JSClassHead {
				body: [
					JSClassMethod {
						kind: "method"
						key: JSStaticPropertyKey {
							value: JSIdentifier {
								name: "a"
								loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:9-1:10 (a)
							}
							loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:9-1:10
						}
						meta: JSClassPropertyMeta {
							abstract: false
							declare: false
							optional: false
							readonly: false
							static: false
							loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:9-1:10
							start: Position 1:9
						}
						body: JSBlockStatement {
							body: []
							directives: []
							loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:12-1:14
						}
						head: JSFunctionHead {
							async: false
							generator: false
							hasHoistedVars: false
							params: []
							loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:10-1:12
						}
						loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:9-1:14
					}
					JSClassMethod {
						kind: "method"
						key: JSStaticPropertyKey {
							value: JSIdentifier {
								name: "b"
								loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:15-1:16 (b)
							}
							loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:15-1:16
						}
						meta: JSClassPropertyMeta {
							abstract: false
							declare: false
							optional: false
							readonly: false
							static: false
							loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:15-1:16
							start: Position 1:15
						}
						body: JSBlockStatement {
							body: []
							directives: []
							loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:18-1:20
						}
						head: JSFunctionHead {
							async: false
							generator: false
							hasHoistedVars: false
							params: []
							loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:16-1:18
						}
						loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:15-1:20
					}
				]
				loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:0-1:21
			}
			loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:0-1:21
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
				message: RAW_MARKUP {value: "Expected an identifier"}
			}
			location: {
				language: "js"
				path: UIDPath<esprima/invalid-syntax/migrated_0269/input.js>
				end: Position 1:14
				start: Position 1:14
			}
		}
	]
	directives: []
	hasHoistedVars: false
	sourceType: "script"
	syntax: []
	path: UIDPath<esprima/invalid-syntax/migrated_0269/input.js>
	loc: SourceLocation esprima/invalid-syntax/migrated_0269/input.js 1:0-2:0
}
```

### `diagnostics`

```

 esprima/invalid-syntax/migrated_0269/input.js:1:14 parse(js) ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Expected an identifier

    class A {a(){},b(){}}
                  ^


```
