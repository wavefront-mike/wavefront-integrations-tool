## Overview
The `wavefront` script facilitates external integrations with Wavefront.  Each new integration is built as a subcommand of the `wavefront` command script.  `wavefront` provides a framework to quickly build new subcommands.  The framework supports several common features:

* daemonize
* PID file creation
* multiple command parallel processing
* continuous execution with delay between each run
* execute command(s) via command line or configuration file

## Existing Commands
| Command Name | Description | Python File |
| ------------ | ----------- | ----------- |
| [newrelic](docs/README.newrelic.md) | New Relic metrics imported into Wavefront.  Additionally, supports executing insight queries. | [newrelic.py](wavefront/newrelic.py) |
| [awsmetrics](docs/README.awsmetrics.md) | AWS Cloudwatch metrics | [awsmetrics.py](wavefront/awsmetrics.py) |
| [systemchecker](docs/README.system_checker.md) | System Checker sends events to Wavefront when core dump files are found or when files have changed | [system_checker.py](wavefront/system_checker.py) |

