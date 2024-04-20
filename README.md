#A Python Get PHP AST 


#install 
```bash
    pip install php_ast
```


#exapme 
```Python
# get phpinfo ast
from php_ast import get_ast
get_ast(b"<?php7 phpinfo();?>")
{'status': 'successed', 'ast': {'kind': 'AST_STMT_LIST', 'flags': 0, 'lineno': 1, 'children': [{'kind': 'AST_CALL', 'flags': 0, 'lineno': 1, 'children': {'expr': {'kind': 'AST_NAME', 'flags': 1, 'lineno': 1, 'children': {'name': 'phpinfo'}}, 'args': {'kind': 'AST_ARG_LIST', 'flags': 0, 'lineno': 1, 'children': []}}}]}}

```

```Python
from php_ast import get_file_ast
get_file_ast("/home/11.php7")
{'status': 'successed', 'ast': {'kind': 'AST_STMT_LIST', 'flags': 0, 'lineno': 1, 'children': [{'kind': 'AST_CALL', 'flags': 0, 'lineno': 1, 'children': {'expr': {'kind': 'AST_NAME', 'flags': 1, 'lineno': 1, 'children': {'name': 'phpinfo'}}, 'args': {'kind': 'AST_ARG_LIST', 'flags': 0, 'lineno': 1, 'children': []}}}]}}

```


