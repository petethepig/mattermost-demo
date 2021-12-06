This is an example of running [mattermost](https://github.com/mattermost/mattermost-server/) with [pyroscope](https://github.com/pyroscope-io/pyroscope/) in pull mode via docker-compose.

### Usage:
```bash
# this will start mattermost-preview docker container and pyroscope-server in pull mode
docker-compose up
```

### Analysing Data

* Open [http://localhost:8065](http://localhost:8065) to access mattermost server
* Open [http://localhost:4040](http://localhost:4040) to access pyroscope server

It will take about a minute for profiling data to start flowing but if it all works correctly you should see mattermost application data in pyroscope:

![Screen Shot 2021-12-06 at 2 34 34 PM](https://user-images.githubusercontent.com/662636/144933713-f080cc6c-a35d-45c4-bd7d-5ac556a107f2.png)


### Profile Example

![flamegraph_visual_06_11_2021](https://user-images.githubusercontent.com/662636/144938200-2c664712-9a86-45a4-a230-5276bac53201.png)
