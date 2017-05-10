# Example config for s3cmd

## Getting s3cmd

Most linux distributions will have s3cmd in their repos, so a simple "apt-get install s3cmd" or "yum install s3cmd" should suffice.

## Creating a config file

s3cmd can be told to output a file containing all options in their current state, but it holds a lot of unneeded information so a simple start config could be as short as:

$HOME/.s3cfg

```[default]
access_key = REDACTED
secret_key = REDACTED
check_ssl_certificate = True
guess_mime_type = True
host_base = s3-archive.api.cloud.ipnett.se
multipart_chunk_size_mb = 16
use_https = True
```

and nothing else.