---
views:
    flash:
        region: flash
        template: anax/v2/image/default
        data:
            #src: "image/theme/tree.jpg?width=1100&height=150&crop-to-fit&area=0,0,30,0"
            src: "image/theme/flash-about.jpg?width=1100&height=150&crop-to-fit&area=0,0,50,0"

    kursrepo:
        region: sidebar-left
        template: anax/v2/block/default
        data:
            meta: 
                type: single
                route: block/om-kursrepo

    redovisa:
        region: sidebar-right
        template: anax/v2/block/default
        data:
            meta: 
                type: single
                route: block/om-redovisa
---
# Test

Testpage 

## Lista
- Foo
- Bar
- Baz

## Codeblock

```python
def main():
    pass
```


