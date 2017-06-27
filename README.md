# btc-crawl

Bitcoin node network crawler (written in golang).

Current status: 
* JSON streaming is in place, and graceful shutdown.

TODO - Log all this data into excel, run at several instances over SCHAMIA etc


## Usage

```
$ btc-crawl \
  --concurrency=100 \
  --output="btc-crawl.json" \
  --peer-age="24h" \
  --user-agent="/batman:1.0/" \
  --verbose
...
```

**Estimated crawl time:**
Each node returns around ~2,500 known nodes, but usually only several have timestamps within the last hour.
Current node list around 6,000

