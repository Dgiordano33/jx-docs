---
date: 2019-05-18T17:53:25Z
title: "jx prompt"
slug: jx_prompt
url: /commands/jx_prompt/
---
## jx prompt

Generate the command line prompt for the current team and environment

### Synopsis

Generate a command prompt for the current namespace and Kubernetes context.

```
jx prompt [flags]
```

### Examples

```
  # Generate the current prompt
  jx prompt
  
  # Enable the prompt for bash
  PS1="[\u@\h \W \$(jx prompt)]\$ "
  
  # Enable the prompt for zsh
  PROMPT='$(jx prompt)'$PROMPT
```

### Options

```
      --context-color stringArray     The color for the Kubernetes context (default [cyan])
  -d, --divider string                The divider between the team and environment for the prompt (default ":")
  -h, --help                          help for prompt
  -i, --icon                          Uses an icon for the label in the prompt
  -l, --label string                  The label for the prompt (default "k8s")
      --label-color stringArray       The color for the label (default [blue])
      --namespace-color stringArray   The color for the namespace (default [green])
      --no-label                      Disables the use of the label in the prompt
  -p, --prefix string                 The prefix text for the prompt
  -s, --separator string              The separator between the label and the rest of the prompt (default ":")
  -x, --suffix string                 The suffix text for the prompt (default ">")
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

* [jx](/commands/jx/)	 - jx is a command line tool for working with Jenkins X

###### Auto generated by spf13/cobra on 18-May-2019