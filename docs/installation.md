# Installation

Installing `kafka-gitops` requires either **Java** or **Docker**.

## Homebrew

Install `kafka-gitops` with homebrew:

```bash
brew tap devshawn/kafka-gitops
brew install kafka-gitops
```

## Local

Install `kafka-gitops` by downloading the zip file from our [releases][releases] page. Move the `kafka-gitops` file to somewhere on your `$PATH`, such as `/usr/local/bin`. 


Ensure the command is working by running:

```bash
kafka-gitops
```

You should see output similar to the following:

```text
Usage: kafka-gitops [-hvV] [--no-delete] [-f=<file>] [COMMAND]
Manage Kafka resources with a desired state file.
  -f, --file=<file>   Specify the desired state file.
  -h, --help          Display this help message.
      --no-delete     Disable the ability to delete resources.
  -v, --verbose       Show more detail during execution.
  -V, --version       Print the current version of this tool.
Commands:
  account   Create Confluent Cloud service accounts.
  apply     Apply changes to Kafka resources.
  plan      Generate an execution plan of changes to Kafka resources.
  validate  Validates the desired state file.
```

## Docker

We provide a public docker image: [joschi/kafka-gitops][docker].

[releases]: https://github.com/joschi/kafka-gitops/releases
[docker]: https://github.com/joschi/kafka-gitops/pkgs/container/kafka-gitops
