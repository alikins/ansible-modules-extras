Contributing to ansible-modules-extras
======================================

The Ansible Extras Modules are written and maintained by the Ansible community, according to the following contribution guidelines. 

How to get a new module into ansible-modules-extras
========================================
Ansible welcomes new modules. Having a wide variety of modules available is a goal of the Ansible project.

Minimal requirements:
---------------------

* The module needs to meet the [module development guide and standards](http://docs.ansible.com/developing_modules.html), including:
  * [Documentation](http://docs.ansible.com/ansible/developing_modules.html#id16)
  * Following standards for naming of arguments and options and the module itself.
  * The module needs to support idempotent operations.
  * The module needs to support 'check' and 'diff' modes.

* The module needs to have a maintainer.
  The maintainers responsiblities include:
  * Reviewing pull requests from other contributors.
  * Approving pull requests for inclusion in releases.
  * Responding to issues related to the module.
  
Recommended requirements:
------------------------

* The module should be testable, and those tests need to be included into the ansible code base.
* The module is well documented. Including:
   * All of the module options, what they mean, default values, and how they interact.
   * All of the options need to include a 'version_added' doc string.
   * As many real world examples of the use of the module as possible.
   * If the module is an interface to an existing tool, the module documention should explain how the module options relate to the existing tool. If there is a cli tool thats equilivant, include examples of the cli invocation that matches the example.
   * Explain any assumptions the module makes and explain why default values are the default.
   * Explain the environment the module is used in.
    * What operating systems are supported.
    * What external software is required.
    * What permissions and access are required.
    * If the module is specific to a user of particular vendors, explain that.
    * If the module is for a specific cloud provider, explain that.

Gold start requirements:
------------------------
* Module is tested and review upstream as well.
* A Continous Integration environment is provided to allow the Ansible project to test the module. Especially if:
 * Testing requires specialized hardware or software.
 * Testing requires access to particular vendors equipment or network.
 * Testing requires propietary software or hardware.
 * Testing requires access to private network, or credentials that are not readily available.
 * Testing requires paying for a service.
* A security contact is provided for timely responses to security issues.

Each new module requires two current module owners to approve a new module for inclusion.  The Ansible community reviews new modules as often as possible, but please be patient; there are a lot of new module submissions in the pipeline, and it takes time to evaluate a new module for its adherence to module standards.

Once your module is accepted, you become responsible for maintenance of that module, which means responding to pull requests and issues in a reasonably timely manner. 

If you'd like to contribute code
================================

Please see [this web page](http://docs.ansible.com/community.html) for information about the contribution process. Important license agreement information is also included on that page.

If you'd like to contribute code to an existing module
======================================================
Each module in Extras is maintained by the owner of that module; each module's owner is indicated in the documentation section of the module itself. Any pull request for a module that is given a "shipit" by the owner in the comments will be merged by the Ansible team.



If you'd like to ask a question
===============================

Please see [this web page ](http://docs.ansible.com/community.html) for community information, which includes pointers on how to ask questions on the [mailing lists](http://docs.ansible.com/community.html#mailing-list-information) and IRC.  

The Github issue tracker is not the best place for questions for various reasons, but both IRC and the mailing list are very helpful places for those things, and that page has the pointers to those.

If you'd like to file a bug
===========================

Read the community page above, but in particular, make sure you copy [this issue template](https://github.com/ansible/ansible-modules-extras/blob/devel/.github/ISSUE_TEMPLATE.md) into your ticket description.  We have a friendly neighborhood bot that will remind you if you forget :)  This template helps us organize tickets faster and prevents asking some repeated questions, so it's very helpful to us and we appreciate your help with it.

Also please make sure you are testing on the latest released version of Ansible or the development branch.

Thanks!
