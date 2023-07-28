# Unreleased

Breaking changes:

* Logging to disk is now disabled by default.
  Logs will no longer be written to `$HOME/.mountpoint-s3/` and should be configured using `--log-directory <DIRECTORY>`.
* Bucket options of `--virtual-addressing` is now removed and `--path-addressing` is changed to `--force-path-style`.
  If `--force-path-style` is not provided, addressing style of endpoint will be resolved automatically.
* The `--thread-count` option has been removed and replaced with `--max-threads` which sets the maximum
  number of threads the FUSE daemon will dynamically spawn to handle requests.

Other changes:

* New bucket options of `--transfer-acceleration`, `--dual-stack` and `--fips` has been added.
* ARN is now also supported as <BUCKET_NAME> to mount the corresponding resource using Mountpoint.

# v0.3.0 (June 30, 2023)

Initial change log entry.