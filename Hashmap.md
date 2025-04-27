
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


If you want to check if two HashMaps are exactly equal (same keys, same values):

Map<Integer, String> map1 = new HashMap<>();
Map<Integer, String> map2 = new HashMap<>();

map1.put(1, "one");
map1.put(2, "two");

map2.put(2, "two");
map2.put(1, "one");

boolean areEqual = map1.equals(map2);  // true

equals() internally checks both keys and values.

Order does not matter because HashMap is unordered.

Time complexity: O(n) where n = number of entries.



**Map with key and list of values**
Map<String,List<String>> map = new HashMap();

adding values to the map
map.get(key).add(value);
map.gey(key) gives us the value which is list here and we add value to the list by .add(value)

**Return List of values as list**
return new ArrayList<>(map.values());
