
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


**IMP**


import java.util.*;

public class SortMapByValueDescending {

    public static void main(String[] args) {
        Map<Integer, Integer> map = new HashMap<>();
        map.put(1, 50);
        map.put(2, 10);
        map.put(3, 40);
        map.put(4, 20);

        // Convert to list
        List<Map.Entry<Integer, Integer>> entryList = new ArrayList<>(map.entrySet());

        // Sort by value descending
        entryList.sort((a, b) -> b.getValue().compareTo(a.getValue()));

        // Directly print
        for (Map.Entry<Integer, Integer> entry : entryList) {
            System.out.println(entry.getKey() + " -> " + entry.getValue());
        }
    }
}

//other imp way

List<Map.Entry<Integer, Integer>> entries = new ArrayList<>(freqMap.entrySet());


entries = [
  Map.Entry(key=1, value=3),
  Map.Entry(key=2, value=2),
  Map.Entry(key=3, value=1)
]



entries.get(i)             // gets the i-th Map.Entry from the list
entries.get(i).getKey()    // gets the key (i.e., the number itself)



entries.get(0) -> Entry(1, 3)   // number 1 appears 3 times
.getKey()     -> 1             // we’re extracting just the number
