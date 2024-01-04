Add extra authorized keys for secure shell access here.
Only add the `*.pub` files; *DO NOT ADD THE PRIVATE KEYS*.

For example, if you have two machines you develop on --- call them `laptop` and
`desktop` ---, you can include the `id_laptop.pub` key in this directory on the
`desktop` machine, and vice-versa. The standard build process already takes the
current machine's keys from `$USER_HOME/.ssh`, so you *do not* need to add the
current machine's public key here.

This allows you to write code on multiple machines, and then use any of them to
administer the target devices. You can also add public keys from non-development
machines that need administrative access to the target devices.

The key files in this directory are ignored by version control, so include any
public keys you need for your development environment.
