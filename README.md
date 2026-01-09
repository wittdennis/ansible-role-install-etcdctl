# install_etcdctl

Installs etcdctl

## Requirements

None.

## Role Variables

```yaml
install_etcdctl_version: "v3.6.7" # version of etcd to install

install_etcdctl_url: "https://github.com/etcd-io/etcd/releases/download/{{ install_etcdctl_version }}/etcd-{{ install_etcdctl_version }}-linux-{{ install_etcdctl_arch }}.tar.gz" # url from where to download the etcd files
install_etcdctl_path: "/usr/local/bin/etcdctl" # absolute path where to put etcdctl
install_etcdctl_force_update: false # flag to control if etcdctl should be updated regardless of version
```

## Dependencies

None

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: wittdennis.install_etcdctl }

## License

MIT
