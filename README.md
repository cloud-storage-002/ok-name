# ok-name

```python
def ok_name(name: str) -> str:
    """替换字符串中的特殊字符"""
    name = name.replace('\\', '＼')
    name = name.replace('/', '／')
    name = name.replace(':', '：')
    name = name.replace('*', '⁕')
    name = name.replace('?', '？')
    name = name.replace('"', '”')
    name = name.replace('<', '＜')
    name = name.replace('>', '＞')
    name = name.replace('|', '¦')
    name = re.sub(r'\s+', ' ', name)
    return name
```
