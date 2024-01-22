# Usage

```
pip install -r requirements.txt

cp src/patch/resource.py `pip show bentoml | grep Location | awk -F ': ' '{print $2}'`/bentoml/_internal/

python download_model.py
bentoml serve service:svc

bentoml build --containerize
docker run -p 3000:3000 summarization:latest

``` 
