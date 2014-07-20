==============================================================================
 The Ansible Playbooks for the session of Tokyo Debian Meeting #115 (2014.07)
==============================================================================

Purpose
-------

These playbooks are prepared for the session of Tokyo Debian Meeting #115 (2014.07),
"The Debian packages building systems automatically on Jenkins.;

* Clean building from git repository or source packages with pbuilder and cowbuilder.
* Tesging to install/unstall with lintian.
* Signing with GPG Public key.
* Uploading to local archives managed with reprepro.

Requirements
------------

* Generate a new GNU PGP key pair for reprepro.
* Generate a new SSH public key pair.
* Install packages as follows;

  * ansible (>= 1.5)
  * python-apt

Playbooks
---------

"repo" directory is the playbook for deploying reprepro system.
"ci" directory is the playbook for deploying Jenkins system.

Execute next command under the each directories.::

  $ ansible-playbook -i production site.yaml -K

