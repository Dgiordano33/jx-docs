---
date: 2019-09-24T12:14:34Z
title: "jx gc helm"
slug: jx_gc_helm
url: /commands/jx_gc_helm/
---
## jx gc helm

garbage collection for Helm ConfigMaps

### Synopsis

Garbage collect Helm ConfigMaps.  To facilitate rollbacks, Helm leaves a history of chart versions in place in Kubernetes and these should be pruned at intervals to avoid consuming excessive system resources.

```
jx gc helm [flags]
```

### Examples

```
  jx garbage collect helm
  jx gc helm
```

### Options

```
      --dry-run                      Does not perform the delete operation on Kubernetes
  -h, --help                         help for helm
      --no-backup                    Does not perform the backup operation to store files locally
  -o, --output-dir string            Relative directory to output backup to. Defaults to ./configmaps (default "configmaps")
      --revision-history-limit int   Minimum number of versions per release to keep (default 10)
```

### Options inherited from parent commands

```
  -b, --batch-mode   Runs in batch mode without prompting for user input (default true)
      --verbose      Enables verbose output
```

### SEE ALSO

* [jx gc](/commands/jx_gc/)	 - Garbage collects Jenkins X resources

###### Auto generated by spf13/cobra on 24-Sep-2019