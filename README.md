ansible-wordpress-haproxy
=========================

This [Ansible][ansible] playbook sets up the classic 3-tier Wordpress demo.  It's currently configured to be optimized for LXC containers running Ubuntu 12.04 LTS, but this should be easily adaptable for other configurations.

In order to run this, you can either setup your local LXC environment to match the declarations in `hosts`, or update hosts to match your local environment.

To run, simply install Ansible and run the playbook, site.yaml:
```bash
$ ansible-playbook -i hosts site.yaml

```

Once it's been deployed, point your browser to ${haproxy_node}/blog/ and see if get the Wordpress installation page.

