# Steam
## Crawl all the game data on the Steam store search page. Usage:
```shell
Usage of ./gamepark-craw:
  -concurrency int
        page crawl concurrency (default 1)
  -output string
        output file path (default "steam.tsv")
  -start int
        start page (default 1)
  -target string
        target website, steam/shanguo (default "steam")
```

where `start` means crawl from the first page, `concurrency` means crawl up to 2 pages at the same time, `output` is used to specify the output file, and `target` means the crawl platform.
The game data is stored in `tsv` format, and there are 6 tokens in a row, each token is split by `\t` in the following format:
```shell
Game name \t current price \t original price \t discount range \t picture \t store
```
