#### 检测并打包
```sh
python setup.py check
# 为什么是sdist...
python setup.py sdist build
```


#### 上传到PYPI
需要安装twine
```sh
pip3 install twine
# 安装完成后执行
twine upload dist/*
```


#### 常见问题
1. TypeError: 'module' object is not callable

