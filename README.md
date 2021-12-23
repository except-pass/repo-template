# Repo Template
> Starting a new python project?  Start with this template.

Clone then edit the `settings.ini`

If you're going to make your own github repo, first you need to remove the existing `.git` folder.

```
rm -rf .git
git init
```

Put your custom code in jupyter notebooks in the `nbs/` folder.  It is helpful to include this boilerplate at the top of each notebook.


```
# default_exp <notebook name>
# hide
_FNAME='<notebook name>'
import unittest
from unittest import mock
from nbdev.export import notebook2script
import os

TESTCASE = unittest.TestCase()
_nbpath = os.path.join(_dh[0], _FNAME+'.ipynb')
notebook2script(_nbpath)
```


