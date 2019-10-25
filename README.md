### renpy
---
https://github.com/renpy/renpy

https://www.renpy.org/

```py
// unittests/testsyles.py

class TestSytles(unittest.TestCase):
  
  def test_set_prefix(self):
    s = Style(None)
    
    s.bold = "insensitive"
    s.hover_bold = "hover"
    s.selected_bold = "selected"
    s.selected_hover_bold = "selected_hover"
    
    renpy.styleaccel.build_style(s)
    
    assert s.bold == "insensitive"
    
    s.set_prefix("hover_")
    assert s.bold == "hover"
    
    s.set_prefix("selected_idle_")
    assert s.bold == "selected"
    
    s.set_prefix("selected_idle_")
    assert s.bold == "selected"
    
    s.set_prefix("insensitive")
    assert s.bold == "insensitve"
  
  def test_inheritance(self):

```

```
```

```
```


