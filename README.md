# jsel (JSON Selector)

jsel is a command-line utility which allows you to extract specific content from a json blob.

## Usage 

Selects a field from a JSON object using dot notation. For example, if
foo.json is:

```json
{
    "myDict": {
        "MyKey": "myValue"
    },
    "AnotherKey": "anotherValue"
    
}
```

Allows you to select values, for example:

```
cat foo.json | jsel myDict.MyKey  # myValue
cat foo.json | jsel AnotherKey  # anotherValue
```

