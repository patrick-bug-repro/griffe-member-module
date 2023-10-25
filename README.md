# Reproduction for members being overridden by modules

```bash
griffe dump strawberry
```

Returns:

```json
{
  "strawberry": {
    "kind": "module",
    "name": "strawberry",
    "labels": [],
    "members": [
      {
        "kind": "module",
        "name": "type",
        "labels": [],
        "members": [
          {
            "kind": "function",
            "name": "hello",
            "lineno": 1,
            "endlineno": 2,
            "labels": [],
            "members": [],
            "decorators": [],
            "parameters": [],
            "returns": null
          }
        ],
        "filepath": "strawberry/type/__init__.py"
      }
    ],
    "filepath": "strawberry/__init__.py"
  }
}
```

But it doesn't include `type` inside `strawberry/__init__.py`
