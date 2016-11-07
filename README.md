# registry-conf

Simple [Docker Registry](https://docs.docker.com/registry/) configuration generator to use as sidekick container.


## Usage

```bash
$ docker run -it \
    -e STORAGE_S3_ACCESSKEY="" \
    -e STORAGE_S3_SECRETKEY="" \
    -e STORAGE_S3_REGION="" \
    -e STORAGE_S3_BUCKET="" \
    -e STORAGE_S3_ENCRYPT="true" \
    -e STORAGE_S3_SECURE="true" \
    -e STORAGE_S3_V4AUTH="true" \
    -e STORAGE_S3_CHUNKSIZE="5242880" \
    -e STORAGE_S3_ROOTDIRECTORY="/" \
    -e STORAGE_DELETE_ENABLED="false" \
    -e STORAGE_CACHE_BLOBDESCRIPTOR="inmemory" \
    -e HTTP_ADDR=":5000" \
    -e HTTP_TLS_CERTIFICATE="" \
    -e HTTP_TLS_KEY="" \
    -e REPORTING_NEWRELIC_LICENSEKEY="" \
    -e REPORTING_NEWRELIC_NAME="" \
    -e REPORTING_NEWRELIC_VERBOSE="false" \
    marceloalmeida/registry-conf
```

## Contributing

All contributions are welcome, but if you are considering significant changes, please open an issue beforehand and discuss it with us.

## License

MIT. See the `LICENSE` file for more information.
