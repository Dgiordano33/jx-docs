---
date: 2019-05-18T17:53:25Z
title: "jx get quickstartlocations"
slug: jx_get_quickstartlocations
url: /commands/jx_get_quickstartlocations/
---
## jx get quickstartlocations

Display one or more Quickstart Locations

### Synopsis

Display one or more Quickstart Locations for the current Team. 

For more documentation see: https://jenkins-x.io/developing/create-quickstart/#customising-your-teams-quickstarts

```
jx get quickstartlocations [flags]
```

### Examples

```
  # List all the quickstart locations
  jx get quickstartlocations
  
  # List all the quickstart locations via an alias
  jx get qsloc
```

### Options

```
  -h, --help            help for quickstartlocations
  -o, --output string   The output format such as 'yaml'
```

### Options inherited from parent commands

```
  -b, --batch-mode                Runs in batch mode without prompting for user input (default true)
      --install-dependencies      Enables automatic dependencies installation when required
      --log-level string          Sets the logging level (panic, fatal, error, warning, info, debug) (default "info")
      --no-brew                   Disables brew package manager on MacOS when installing binary dependencies
      --skip-auth-secrets-merge   Skips merging the secrets from local files with the secrets from Kubernetes cluster
      --verbose                   Enables verbose output
```

### SEE ALSO

* [jx get](/commands/jx_get/)	 - Display one or more resources

###### Auto generated by spf13/cobra on 18-May-2019