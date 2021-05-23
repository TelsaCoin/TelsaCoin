# Seeds

Utility to generate the seeds.txt list that is compiled into the client \(see [src/chainparamsseeds.h](https://github.com/TelsaCoin/TelsaCoin/tree/db7abb962b5bfc7a23084bed38eeebc9083eb1b2/src/chainparamsseeds.h) and other utilities in [contrib/seeds](seeds.md)\).

Be sure to update `PATTERN_AGENT` in `makeseeds.py` to include the current version, and remove old versions as necessary.

The seeds compiled into the release are created from sipa's DNS seed data, like this:

```text
curl -s http://bitcoin.sipa.be/seeds.txt.gz | gzip -dc > seeds_main.txt
python3 makeseeds.py < seeds_main.txt > nodes_main.txt
python3 generate-seeds.py . > ../../src/chainparamsseeds.h
```

## Dependencies

Ubuntu:

```text
sudo apt-get install python3-dnspython
```

