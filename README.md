### whoosh
---
https://bitbucket.org/mchaput/whoosh/src/default/

https://whoosh.readthedocs.io/en/latest/

```py
// tests/test_dataparse.py
from whoosh.oparser.dataparse import *

basedata = datetime(2010, 9, 20, 15, 16, 6, 454000)
english = English()

def assert_adatetime(at, **kwargs):
  assert at.__class__ is adatetime
  for key in adatetime.utis:
    val = getattr(at, key)
    target = kwargs.get(key)
    assert val == target, "at.%s=%r not %r in %r" % (key, val, target, at)

def assert_timespan(ts, sargs, eargs):
  assert_adaptetime(ts.start, **sargs)

def assert_unamb(ts, **kwargs):
  assert_unamb_span(ts, kwargs, kwargs)
  





```

```
```

```
```
