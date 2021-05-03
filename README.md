# AR Cut Paste local server

## Setup

```bash
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Run

The `BASNET_SERVICE_HOST` is optional (only needed if you've deployed the service
on a platform using an ingress gateway such as Knative / Cloud Run).

Replace `123456` by your Photoshop remote connection password.

```python
python src/main.py \
    --basnet_service_ip="http://X.X.X.X" \
    --basnet_service_host="basnet-http.default.example.com" \
    --photoshop_password 123456
```
