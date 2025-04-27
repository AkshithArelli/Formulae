
| Function | Usage | Purpose |
|:---------|:------|:--------|
| `put(K key, V value)` | `map.put(1, "one");` | Insert or update key-value pair |
| `get(K key)` | `map.get(1);` | Retrieve value for a key |
| `containsKey(K key)` | `map.containsKey(1);` | Check if a key exists |
| `containsValue(V value)` | `map.containsValue("one");` | Check if a value exists |
| `remove(K key)` | `map.remove(1);` | Remove key-value by key |
| `size()` | `map.size();` | Get number of key-value pairs |
| `isEmpty()` | `map.isEmpty();` | Check if map is empty |
| `keySet()` | `map.keySet();` | Get set of all keys |
| `values()` | `map.values();` | Get collection of all values |
| `entrySet()` | `map.entrySet();` | Get set of key-value entries (handy for iterating) |
| `getOrDefault(K key, V defaultValue)` | `map.getOrDefault(1, "default");` | If key exists, return value; else return default |
| `putIfAbsent(K key, V value)` | `map.putIfAbsent(1, "one");` | Only put if key is not already present |
