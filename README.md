# prometheus-for-beginners

This is the companion repo for the "Prometheus for Beginners" YouTube video.


## Usage

First download and extract the Prometheus binary for your platform from [here](https://github.com/prometheus/prometheus/releases).

Now start up the server which we use to generate the metrics (which Prometheus will scrape):
```
pip install -r requirements.txt
fastapi dev main.py --port 9123
```

Now start prometheus:

```
./prometheus --config.file=prometheus.yml
```
