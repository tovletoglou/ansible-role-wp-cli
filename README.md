# Ansible Role: WP-CLI

Installs WP-CLI, a command line shell and scripting interface for Wordpress

## Requirements

Tested on RedHat & CentOS 7

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

WP-CLI phar URL.

```yml
wp_cli_phar_url: https://raw.github.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
```

The location of the wp-cli installation.

```yml
wp_cli_path: /usr/local/bin/wp
```

Update WP-CLI every time we run the role.

```yml
wp_cli_keep_updated: yes
```

## Dependencies

None

## Example Playbook

Call the role with the default variables

```yml
- hosts: servers
  roles:
    - ansible-role-wp-cli
```

After the playbook runs, the `wp` command will be accessible from normal system accounts.

## License

MIT
