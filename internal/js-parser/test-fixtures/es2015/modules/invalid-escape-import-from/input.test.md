# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `es2015 > modules > invalid-escape-import-from`

### `ast`

```javascript
JSRoot {
	body: [
		JSImportDeclaration {
			namedSpecifiers: []
			defaultSpecifier: JSImportDefaultSpecifier {
				local: JSImportSpecifierLocal {
					name: JSBindingIdentifier {
						name: "X"
						loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:7-1:8 (X)
					}
					loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:7-1:8
				}
				loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:0-1:8
			}
			source: JSStringLiteral {
				value: ""
				loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:0-1:8
			}
			loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:0-1:8
		}
		JSExpressionStatement {
			expression: JSReferenceIdentifier {
				name: "from"
				loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:9-1:18 (from)
			}
			loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:9-1:18
		}
		JSExpressionStatement {
			expression: JSStringLiteral {
				value: "x"
				loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:19-1:22
			}
			loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:19-1:22
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
				message: [RAW_MARKUP {value: "Expected keyword <emphasis>"}, "from", RAW_MARKUP {value: "</emphasis>"}]
			}
			location: {
				language: "js"
				path: UIDPath<es2015/modules/invalid-escape-import-from/input.js>
				end: Position 1:9
				start: Position 1:9
			}
		}
	]
	directives: []
	hasHoistedVars: false
	sourceType: "script"
	syntax: []
	path: UIDPath<es2015/modules/invalid-escape-import-from/input.js>
	loc: SourceLocation es2015/modules/invalid-escape-import-from/input.js 1:0-2:0
}
```

### `diagnostics`

```

 es2015/modules/invalid-escape-import-from/input.js:1:9 parse(js) ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Expected keyword from

    import X fro\u006d 'x'
             ^


```
