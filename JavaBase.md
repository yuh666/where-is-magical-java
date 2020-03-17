
### 1.字符串问题
```
String a = new String("a" + "b");
String b = new String("ab");
System.out.println(a == b);
System.out.println(a.intern() == b);
System.out.println(b == b.intern());
System.out.println(a.intern() == b.intern());
```

### 2.浮点数问题
```
System.out.println(1 == 1.0);
System.out.println(1.0F == 1.0D);
System.out.println(1.1F == 1.1D);
```

### 3.迭代器问题
```
List<String> list = new ArrayList<>();
list.add("1");
list.add("2");
list.add("3");
for (String s : list) {
    if (s == "2") {
        list.remove("2");
    }
    System.out.println(s);
}
```
