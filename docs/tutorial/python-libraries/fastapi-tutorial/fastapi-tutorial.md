#

## 官方網站
[https://fastapi.tiangolo.com/]

## 安裝

```bash
pip install "fastapi[standard]"
```

## 測試範例

建立檔案 main.py
```python
from fastapi import FastAPI

app = FastAPI()


@app.get("/")
def read_root():
    return {"Hello": "World"}


@app.get("/items/{item_id}")
def read_item(item_id: int, q: str | None = None):
    return {"item_id": item_id, "q": q}
```

執行
```bash
fastapi dev
```

檢查
[http://127.0.0.1:8000]
API 文件
[http://127.0.0.1:8000/docs]

## 官方教學
[https://fastapi.tiangolo.com/learn/]