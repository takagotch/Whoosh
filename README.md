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
  
def assert_unamb_span(ts, sargs, eargs):
  startdt = adatetime(**sargs).floor()
  enddt = adatetime(**eargs).ceil()
  assert ts.start == startdt, "start %s != %s" % (ts.start, startdt)
  assert ts.end == enddt, "end %s != %s" % (ts.end, enddt)

def assert_datespan(ts, startdate, enddate):
  assert ts.__class__is timespan
  assert ts.start == startdate
  assert ts.end == enddate
  
def test_simple_dateparse(t=english.simple):

def test_all():
  p = english.all
  test_bundle_sups(p)
  test_bundle(p)
  test_ranges(p)
  
def test_final_dates(p=english):

def test_final_ranges(p=english):
```

```
```

```
```
