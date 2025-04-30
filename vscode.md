# VSCode Snippets for React Development

> [!NOTE]
> Allman brace style approach is used.

A collection of handy VSCode snippets to speed up React component creation, including both client and server components with and without props.

## Table of Contents

- [React Client Component](#react-client-component)
- [React Client Component with Props](#react-client-component-with-props)
- [React Server Component](#react-server-component)
- [React Server Component with Props](#react-server-component-with-props)
- [React Action Handler](#react-action-handler)

---

## React Client Component

`rcc`

Basic client-side React component template.

**Snippet:**

```json
"React Client Component": {
    "prefix": "rcc",
    "body": [
        "\"use client\"",
        "",
        "import React from \"react\"",
        "",
        "function ${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}()",
        "{",
        "    return (",
        "        <div>",
        "            $0",
        "        </div>",
        "    )",
        "}",
        "",
        "export default ${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}",
        ""
    ]
}
```

[⬆️ back to top](#vscode-snippets-for-react-development)

---

## React Client Component with Props

`rccp`

Client-side component template with typed props interface.

**Snippet:**

```json
"React Client Component with Props": {
    "prefix": "rccp",
    "body": [
        "\"use client\"",
        "",
        "import React from \"react\"",
        "",
        "interface I${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}Props",
        "{",
        "    $0",
        "}",
        "",
        "function ${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}({",
        "    ",
        "}: I${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}Props)",
        "{",
        "    return (",
        "        <div>",
        "            ",
        "        </div>",
        "    )",
        "}",
        "",
        "export default ${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}",
        ""
    ]
}
```

[⬆️ back to top](#vscode-snippets-for-react-development)

---

## React Server Component

`rsc`

Server-side component without props, for static or data-fetching use cases.

**Snippet:**

```json
"React Server Component": {
    "prefix": "rsc",
    "body": [
        "import React from \"react\"",
        "",
        "function ${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}()",
        "{",
        "    return (",
        "        <div>",
        "            $0",
        "        </div>",
        "    )",
        "}",
        "",
        "export default ${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}",
        ""
    ]
}
```

[⬆️ back to top](#vscode-snippets-for-react-development)

---

## React Server Component with Props

`rscp`

Server-side component with props interface for more complex static or server-rendered UIs.

**Snippet:**

```json
"React Server Component with Props": {
    "prefix": "rscp",
    "body": [
        "import React from \"react\"",
        "",
        "interface I${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}Props",
        "{",
        "    $0",
        "}",
        "",
        "function ${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}({",
        "    ",
        "}: I${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}Props)",
        "{",
        "    return (",
        "        <div>",
        "            ",
        "        </div>",
        "    )",
        "}",
        "",
        "export default ${2:${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/}}",
        ""
    ]
}
```

[⬆️ back to top](#vscode-snippets-for-react-development)

---

## React Action Handler

`rah`

Simple snippet for creating a reusable event handler function.

**Snippet:**

```json
"React Action Handler": {
    "prefix": "rah",
    "body": [
        "function handle$1()",
        "{",
        "    $0",
        "}"
    ]
}
```

[⬆️ back to top](#vscode-snippets-for-react-development)
