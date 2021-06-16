# integrity

[![quality](https://img.shields.io/ansible/quality/27910)](https://galaxy.ansible.com/vbotka/integrity)[![Build Status](https://travis-ci.org/vbotka/ansible-integrity.svg?branch=master)](https://travis-ci.org/vbotka/ansible-integrity)

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


## Variables

See defaults and examples in vars.


## Best practice

Install the roles and collections

```
ansible-galaxy role install vbotka.integrity
ansible-galaxy role install vbotka.ansible_lib
ansible-galaxy collection install community.general
```

Create the playbook and inventory. Check the syntax

```
shell> ansible-playbook integrity.yml --syntax-check
```

Install packages

```
shell> ansible-playbook integrity.yml -t integrity_packages
```

Download source

```
shell> ansible-playbook integrity.yml -t integrity_source
```

Dry-run playbook

```
shell> ansible-playbook integrity.yml --check
```

Run the playbook twice

```
shell> ansible-playbook integrity.yml
```


## References
-----------
- [Path names must by preceded by a period](http://unix.stackexchange.com/questions/316210/mtree8-use-of-o/316614)


## License

[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)


## Author Information

[Vladimir Botka](https://botka.link)
