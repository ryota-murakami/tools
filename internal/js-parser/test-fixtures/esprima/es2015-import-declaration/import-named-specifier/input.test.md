# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `esprima > es2015-import-declaration > import-named-specifier`

### `ast`

```javascript
JSRoot {
	body: [
		JSImportDeclaration {
			namedSpecifiers: [
				JSImportSpecifier {
					imported: JSIdentifier {
						name: "bar"
						loc: SourceLocation esprima/es2015-import-declaration/import-named-specifier/input.js 1:8-1:11 (bar)
					}
					local: JSImportSpecifierLocal {
						name: JSBindingIdentifier {
							name: "bar"
							loc: SourceLocation esprima/es2015-import-declaration/import-named-specifier/input.js 1:8-1:11 (bar)
						}
						loc: SourceLocation esprima/es2015-import-declaration/import-named-specifier/input.js 1:8-1:11
					}
					loc: SourceLocation esprima/es2015-import-declaration/import-named-specifier/input.js 1:8-1:11
				}
			]
			source: JSStringLiteral {
				value: "foo"
				loc: SourceLocation esprima/es2015-import-declaration/import-named-specifier/input.js 1:18-1:23
			}
			loc: SourceLocation esprima/es2015-import-declaration/import-named-specifier/input.js 1:0-1:24
		}
	]
	comments: []
	corrupt: false
	diagnostics: [
		{
			origins: [{entity: "ParserCore<js>"}]
			description: {
				advice: [
					log {
						category: "info"
						text: RAW_MARKUP {value: "Change the extension to <emphasis>.mjs</emphasis> to turn this file into a module"}
					}
					log {
						category: "info"
						text: RAW_MARKUP {value: "Add <emphasis>\"type\": \"module\"</emphasis> to your <filelink emphasis target=\"<dim>undefined</dim>\" />"}
					}
				]
				category: ["parse"]
				categoryValue: "js"
				message: RAW_MARKUP {value: "<emphasis>import</emphasis> and <emphasis>export</emphasis> can only appear in a module"}
			}
			location: {
				language: "js"
				path: UIDPath<esprima/es2015-import-declaration/import-named-specifier/input.js>
				end: Position 1:24
				start: Position 1:0
			}
		}
	]
	directives: []
	hasHoistedVars: false
	sourceType: "script"
	syntax: []
	path: UIDPath<esprima/es2015-import-declaration/import-named-specifier/input.js>
	loc: SourceLocation esprima/es2015-import-declaration/import-named-specifier/input.js 1:0-2:0
}
```

### `diagnostics`

```

 esprima/es2015-import-declaration/import-named-specifier/input.js:1 parse(js) ━━━━━━━━━━━━━━━━━━━━━

  ✖ import and export can only appear in a module

    import {bar} from "foo";
    ^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Change the extension to .mjs to turn this file into a module

  ℹ Add "type": "module" to your <dim>undefined</dim>


```
