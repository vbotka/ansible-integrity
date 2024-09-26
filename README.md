# integrity

[![quality](https://img.shields.io/ansible/quality/27910)](https://galaxy.ansible.com/vbotka/integrity)
[![Build Status](https://app.travis-ci.com/vbotka/ansible-integrity.svg?branch=master)](https://app.travis-ci.com/vbotka/ansible-integrity)
[![GitHub tag](https://img.shields.io/github/v/tag/vbotka/ansible-integrity)](https://github.com/vbotka/ansible-integrity/tags)

[Ansible role](https://galaxy.ansible.com/vbotka/integrity/).
- Install [integrity](https://github.com/vbotka/integrity)
- Record metadata (hash/mtree) of specified directories
- Configure cron to email alerts.

Feel free to [share your feedback and report issues](https://github.com/vbotka/ansible-integrity/issues).

[Contributions are welcome](https://github.com/firstcontributions/first-contributions).


## Requirements

### Roles

* Ansible role [vbotka.ansible_lib](https://galaxy.ansible.com/vbotka/ansible_lib)

### Collections

* community.general


### Packages

* Linux: hashdeep, freebsd-buildutils or mtree-netbsd
* FreeBSD: security/md5deep

Note: RH package *md5deep* provides *hashdeep*. There is no package in RH that provides *fmtree* (searching ... WIP).


## Variables

See defaults and examples in vars.


## Best practice

Install roles

```bash
ansible-galaxy role install vbotka.integrity
ansible-galaxy role install vbotka.ansible_lib
```

Install the collection if necessary

```bash
ansible-galaxy collection install community.general
```

Create the playbook and inventory. Check the syntax

```bash
shell> ansible-playbook integrity.yml --syntax-check
```

Install packages

```bash
shell> ansible-playbook integrity.yml -t integrity_pkg
```

Download source

```bash
shell> ansible-playbook integrity.yml -t integrity_source
```

Dry-run playbook

```bash
shell> ansible-playbook integrity.yml --check
```

Run the playbook twice

```bash
shell> ansible-playbook integrity.yml
```


## Ansible lint

Use the configuration file *.ansible-lint.local* when running
*ansible-lint*. Some rules might be disabled and some warnings might
be ignored. See the notes in the configuration file.

```bash
shell> ansible-lint -c .ansible-lint.local
```


## References

- [Path names must by preceded by a period](http://unix.stackexchange.com/questions/316210/mtree8-use-of-o/316614)


## License

[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)


## Author Information

[Vladimir Botka](https://botka.info)
