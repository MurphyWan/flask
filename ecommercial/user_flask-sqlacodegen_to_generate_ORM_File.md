### 问题：
- windows下使用flask-sqlacodegen，使用总是报错无法生成对应的ORM文件

### 方法：
- windows下先安装pymysql
- 然后在mysql前增加+pymysql
- 另外，mysql这个字符串前后一定要加上英文半角的双引号

### 示例：
```python
flask-sqlacodegen "mysql+pymysql://root:passport@127.0.0.1/food_db" --tables user --outfile "common/models/User.py"  --flask
```
