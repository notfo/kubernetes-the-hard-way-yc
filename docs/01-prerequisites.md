## Yandex Cloud CLI

### Install the Yandex Cloud CLI

Follow the Yandex Cloud CLI [documentation](https://cloud.yandex.com/en/docs/cli/quickstart) to install and configure the `yc` command line utility.

Verify the Yandex Cloud CLI version is 0.98.0 or higher:

```
yc version
```

### Set a Default Compute Region and Zone

This tutorial assumes a default compute region and zone have been configured.

If you are using the `yc` command-line tool for the first time `init` is the easiest way to do this:

```
yc init
```

 View your CLI profile settings:
      ```
      yc config list
      ```


## Running Commands in Parallel with tmux

[tmux](https://github.com/tmux/tmux/wiki) can be used to run commands on multiple compute instances at the same time. Labs in this tutorial may require running the same commands across multiple compute instances, in those cases consider using tmux and splitting a window into multiple panes with synchronize-panes enabled to speed up the provisioning process.

> The use of tmux is optional and not required to complete this tutorial.

![tmux screenshot](images/tmux-screenshot.png)

> Enable synchronize-panes by pressing `ctrl+b` followed by `shift+:`. Next type `set synchronize-panes on` at the prompt. To disable synchronization: `set synchronize-panes off`.

Next: [Installing the Client Tools](02-client-tools.md)
