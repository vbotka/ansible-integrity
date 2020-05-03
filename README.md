# integrity


[![Build Status](https://travis-ci.org/vbotka/ansible-integrity.svg?branch=master)](https://travis-ci.org/vbotka/ansible-integrity)

[Ansible role](https://galaxy.ansible.com/vbotka/integrity/).
- Install *integrity* from [github.com/vbotka/integrity](https://github.com/vbotka/integrity)
- Record metadata (hash/mtree) of specified direcories
- Configure cron to email alerts about inconsistencies.

Please feel free to [share your feedback and report issues](https://github.com/vbotka/ansible-integrity/issues). Contributions are welcome.


## Requirements

None.


## Role Variables

See defaults and examples in vars.


## Dependencies

None.


## Best practice

Check syntax
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
