# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `esprima > invalid-syntax > migrated_0274`

### `ast`

```javascript
JSRoot {
	body: [
		JSClassDeclaration {
			id: JSBindingIdentifier {
				name: "A"
				loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:6-1:7 (A)
			}
			meta: JSClassHead {
				body: [
					JSClassMethod {
						kind: "constructor"
						key: JSStaticPropertyKey {
							value: JSIdentifier {
								name: "constructor"
								loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:9-1:20 (constructor)
							}
							loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:9-1:20
						}
						meta: JSClassPropertyMeta {
							abstract: false
							declare: false
							optional: false
							readonly: false
							static: false
							loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:9-1:20
							start: Position 1:9
						}
						body: JSBlockStatement {
							body: []
							directives: []
							loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:22-1:24
						}
						head: JSFunctionHead {
							async: false
							generator: false
							hasHoistedVars: false
							params: []
							loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:20-1:22
						}
						loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:9-1:24
					}
					JSClassMethod {
						kind: "constructor"
						key: JSStaticPropertyKey {
							value: JSStringLiteral {
								value: "constructor"
								loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:25-1:38
							}
							loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:25-1:38
						}
						meta: JSClassPropertyMeta {
							abstract: false
							declare: false
							optional: false
							readonly: false
							static: false
							loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:25-1:38
							start: Position 1:25
						}
						body: JSBlockStatement {
							body: []
							directives: []
							loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:40-1:42
						}
						head: JSFunctionHead {
							async: false
							generator: false
							hasHoistedVars: false
							params: []
							loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:38-1:40
						}
						loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:25-1:42
					}
				]
				loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:0-1:43
			}
			loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:0-1:43
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
				message: RAW_MARKUP {value: "Duplicate constructor in the same class"}
			}
			location: {
				language: "js"
				path: UIDPath<esprima/invalid-syntax/migrated_0274/input.js>
				end: Position 1:38
				start: Position 1:25
			}
		}
	]
	directives: []
	hasHoistedVars: false
	sourceType: "script"
	syntax: []
	path: UIDPath<esprima/invalid-syntax/migrated_0274/input.js>
	loc: SourceLocation esprima/invalid-syntax/migrated_0274/input.js 1:0-2:0
}
```

### `diagnostics`

```

 esprima/invalid-syntax/migrated_0274/input.js:1:25 parse(js) ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Duplicate constructor in the same class

    class A {constructor(){} "constructor"(){}}
                             ^^^^^^^^^^^^^


```
