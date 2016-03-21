# `invocare.ssh`

Python [`invoke`](http://www.pyinvoke.org/) tasks for SSH activities.

## `ssh_run`

Runs a command on a host via SSH.  For example, running `ls -la` on `www.foo.com`:

```sh
$ invoke ssh_run www.foo.com 'ls -la'
```

Default options for this task may be set within the `ssh` configuration context.

## `ssh_hostkey_remove`

Removes a SSH host key from a user's known hosts.  For example, removing the host key for `www.foo.com`:

```sh
$ invoke ssh_hostkey_remove www.foo.com
```

Default options for this task may be set within the `ssh_hostkey` configuration context.
