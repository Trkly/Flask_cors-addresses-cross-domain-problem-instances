# Flask_cors-addresses-cross-domain-problem-instances
## 安装flask_cors
```
pip install flask_cors
```

## 后端返回
```
from flask import Flask
from flask_cors import cross_origin

app = Flask(__name__)


@app.route('/zzk', methods=['POST', 'GET'])
@cross_origin(origins="http://localhost:8081")  # 设置可以访问的前端端口
def hello_world():
    return 'ZZK TXDY '


if __name__ == '__main__':
    app.run(debug=True)

```
## 前端获取
![](https://img2020.cnblogs.com/blog/2006461/202107/2006461-20210726092946946-22267919.png)

## Github仓库
相关代码我已经放到了Github，欢迎Star  
仓库地址：https://github.com/Trkly/Flask_cors-addresses-cross-domain-problem-instances
