# Usage

```
pip install -r requirements.txt

sudo apt update && sudo apt install patch -y

patch `pip show bentoml | grep Location | awk -F ': ' '{print $2}'`/bentoml/_internal/resource.py patch.diff

python download_model.py
bentoml serve service:svc

bentoml build --containerize
docker run -p 3000:3000 summarization:latest

``` 